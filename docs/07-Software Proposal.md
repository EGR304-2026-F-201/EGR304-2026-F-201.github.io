---
title: Fill-A-Bot Software Proposal
---

## Introduction

This Fill-A-Bot prototype will make use of rudimentary two-wire four-state I/O to transfer data between the subsystems. Each subsystem will continuously monitor its respective inputs and only stop monitoring the inputs when it meets a set criteria and then outputs the necessary state. Currently, we have yet to write this program, but have a proposal in the form of a Flow Chart.

## Research Question

* Will our design have issues in regards to timing?
* How simple can we make this program?
* Will 4 states per I/O be enough to make this system work?

## Images


![Program Flow Chart](https://raw.githubusercontent.com/EGR304-2026-F-201/EGR304-2026-F-201.github.io/refs/heads/main/docs/Appendix/FillABot_Function_Flow.drawio.png){style width:"350" height:"300;"}
**Figure 1:** Our flow chart from which we will be basing our code.



## Rationale

The reason we went with this proposed system flow is because we were no longer using a serial bus protocol. We were confused by some of the instructions in the assignments that specified the use of UART. However after realizing we could use logic states put on the pins. After analyzing the various cases of use for this device, we elected that we could use two wires per "port" giving us a total of four states to work with. When divising the flow chart, we kept these features in mind. Since we were working with a four state communication line, we had to change our previous idea of the user entering an integer value and unit of the amount they wanted to merely 4 preset options. This would allow the scale board to know the amount the user selected while using such a primitive method for data transfer. 

## Results

Yet to be determined!

## Conclusions and Future Work

Yet to be determined!

## External Links

Yet to be determined!


## References


