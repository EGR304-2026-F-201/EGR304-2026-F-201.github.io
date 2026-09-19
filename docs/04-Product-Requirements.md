---
title: Product Requirements
---

## Project Objective
The objective of Fill-A-bot is to develop a reliable liquid dispensing system that gives engineering students and technicians a faster and more consistent way to measure and dispense liquids. The main purpose of the product is to reduce the amount of manual measuring required while also improving repeatability, reducing spills, and clearly showing the user how much liquid has been delivered.
Fill-A-Bot should allow a user to request a desired amount of liquid, dispense that amount within an acceptable level of accuracy, and stop the dispensing process once the target has been reached. The system should be simple enough to operate with minimal instruction and reliable enough to complete repeated dispensing cycles without frequent resets or re-calibration. The final product should also be practical for use on a laboratory bench or similar work area. It should be compact, easy to maintain, and designed so that liquid is kept away from sensitive electronics during normal operation. The product should use components and manufacturing methods that are realistic for the team to obtain, assemble, test, and maintain within the semester. Success for Fill-A-Bot will be based on its ability to repeatedly dispense selected quantities of liquid, provide clear feedback to the user, minimize spills and leaks, and operate safely and consistently through normal use.


## Stakeholders

* **Target group** Professors, students, technicians, and other users who need to dispense measured amounts of liquid quickly and consistently. Their main needs are accuracy, repeatability, ease of use, and less manual measuring.
* **Target purchaser** Schools, laboratories, engineering teams, or other organizations that may need a reliable liquid dispensing system. They would likely focus on cost, reliability, and ease of maintenance.
* **Maintenance / Service** Users responsible for cleaning, troubleshooting, or replacing parts. They need the liquid-contacting parts to be easy to access, clean, and replace without taking apart the entire system.
* **Marketing & Sales** Would focus on the main advantages of Fill-A-Bot, such as repeatable dispensing, simple operation, reduced manual measuring, and less mess during use.
* **Retailers / Distributors** Would care about the product being compact, durable, easy to package, and able to handle normal shipping and storage conditions without damage.

## Use Cases

### User Story #1: Maya – Engineering Student

Maya is an engineering student working in a laboratory and needs 250 mL of water for an experiment. Instead of measuring the liquid manually, she places her container under Fill-A-Bot, selects the amount she needs, and starts the system. Fill-A-Bot dispenses the water while showing the amount being delivered and automatically stops when the selected amount is reached.

Later, Maya needs a different amount of water for another test, so she enters a new quantity and repeats the process. The system gives her consistent measurements, reduces the chance of spills, and works with different containers. After she is finished, the liquid-contacting parts are easy to clean so the system can be ready for the next use.

### User Story #2: Jordan – Home User

Jordan is preparing a recipe at home that requires a specific amount of water. Instead of using a measuring cup and checking the level by hand, Jordan places a container under Fill-A-Bot, enters the amount needed, and starts the system. The dispenser releases the selected amount of water and automatically stops once the target is reached.

Later in the day, Jordan uses Fill-A-Bot again to fill a bottle with a different amount of water. The system makes it easier to get consistent amounts without overfilling the container or spilling water on the counter. Its simple controls make it useful for normal everyday tasks around the house.

## Aspects

The following requirements describe the expected performance and features of Fill-A-Bot. The **P1 - P10** code indicates the priority of each requirement, from low to high, with **P10 representing the highest priority**.

### 1. Hardware / Product Design

* **1.1** The product shall measure the amount of liquid being dispensed with sufficient accuracy to meet the specified dispensing tolerance. (P10)
* **1.2** The product shall automatically start and stop liquid flow during a dispensing cycle. (P10)
* **1.3** The dispensing area shall accommodate multiple common container sizes. (P8)
* **1.4** The product shall remain stable during normal dispensing operations. (P9)
* **1.5** The product shall keep liquid away from exposed electrical components during normal operation. (P10)
* **1.6** Components requiring routine cleaning or maintenance shall be accessible without complete disassembly of the product. (P7)

### 2. Software / Functionality

* **2.1** The product shall allow the user to select a desired quantity of liquid before dispensing. (P10)
* **2.2** The system shall monitor the quantity of liquid delivered during a dispensing cycle. (P10)
* **2.3** The product shall automatically stop dispensing when the target quantity has been reached within the specified tolerance. (P10)
* **2.4** The product shall allow repeated dispensing cycles without requiring a system restart between cycles. (P9)
* **2.5** The system shall provide a method for calibration or zeroing of the measurement system. (P9)
* **2.6** The system shall prevent unintended continuous dispensing after a dispensing cycle is complete. (P10)

### 3. Interactivity & User Experience

* **3.1** The user shall be able to select the desired dispensing quantity using the product controls. (P10)
* **3.2** The product shall clearly communicate the selected dispensing quantity to the user. (P9)
* **3.3** The product shall provide feedback while a dispensing cycle is active. (P8)
* **3.4** The product shall clearly indicate when a dispensing cycle is complete. (P9)
* **3.5** A first-time user shall be able to complete a normal dispensing operation using provided instructions without assistance. (P8)
* **3.6** Displayed measurements and system messages shall be readable from the normal operating position. (P8)

### 4. Customization

* **4.1** The product shall allow users to select multiple dispensing quantities. (P9)
* **4.2** Dispensing quantities shall be configurable without requiring changes to the primary hardware. (P6)
* **4.3** The measurement system shall provide a calibration or zeroing function. (P8)
* **4.4** The design should allow future support for additional measurement units or dispensing settings. (P4)

### 5. Manufacturing

* **5.1** The prototype shall primarily use commercially available components when practical. (P7)
* **5.2** The design shall minimize unnecessary mechanical complexity and moving parts. (P6)
* **5.3** Electrical and mechanical connections shall remain secure during repeated normal operation. (P9)
* **5.4** Components requiring replacement or maintenance should be accessible using common tools. (P6)
* **5.5** Major reusable components shall be capable of being assembled and disassembled without permanent damage. (P5)
* **5.6** Materials exposed to liquid shall be suitable for repeated contact with the intended liquid during prototype operation. (P9)

### 6. Safety

* **6.1** The product shall provide a method for the user to stop dispensing before a normal dispensing cycle is complete. (P10)
* **6.2** Liquid shall be physically separated from exposed electrical connections during normal operation. (P10)
* **6.3** The product shall minimize leakage and splashing during normal dispensing. (P10)
* **6.4** The system shall stop liquid flow after completing a dispensing cycle. (P10)
* **6.5** The product shall remain stable and shall not tip during normal operation with supported containers. (P9)
* **6.6** User-accessible surfaces shall not contain sharp edges that present a cutting hazard during normal use. (P8)
* **6.7** Electrical components shall operate within their manufacturer-specified voltage and current limits. (P10)
## Requirement Criteria Specifications

### Design Requirements

#### 1. Functional Requirements

* **1.1** *Fill Method:* The device must transfer liquid from a source to a desired container using an electric pump. 
* **1.2** *Use of Logic:* The device must use a microcontroller to measure the amount of liquid being dispensed.
* **1.3** *Accuracy:* The device must fill containers to +-1% the desired amount.
* **1.4** *Units:* The device must be able accurately fill using different user-specified units.
* **1.5** *Emergency Stop:* The device must be able to be stopped at any moment by the user. 
* **1.6** *Water-Tightness:* The device must not leak when both idle and operating. 

#### 2. Software/UI Requirements

* **2.1** *Display:* The device must use a display that tells the user the numerical amount entered as well as the specified units. The display must also show the status of the device such as "Ready", "Filling", and "Finished". 
 * **2.2** *Unit Calculations:* The device must make calculations to determine how to much to fill a container when using differing units. 
* **2.3** *Responsiveness:* The device must give user a positve confirmation that their input has been recognized by the device. 
* **2.4** *User Input*: The device must have a physical means for user input on the device itself. 

#### 3. User Experience Requirements

* **3.1** *Ease of Use:* A first-time user provided with operating instructions shall be able to complete one normal dispensing cycle without assistance.  
  **Verification:** Demonstration

* **3.2** *Container Compatibility:* The device shall accommodate at least two different container sizes without modification to the primary dispensing hardware.  
  **Verification:** Demonstration

* **3.3** *Readability:* Displayed quantities and system status information shall be readable from the normal operating position.  
  **Verification:** Inspection

* **3.4** *Manual Stop:* The user shall be able to manually stop an active dispensing cycle using a user-accessible control.  
  **Verification:** Demonstration

#### 4. Hardware Requirements

* **4.1** *Microcontroller:* The device must make use of the PIC18F57Q43 Curiosity Nano Board. 
* **4.2** *Display:* The device must use a high-contrast easy-to-read display. 




## Open Questions

* What range of liquid volumes should Fill-A-Bot be able to dispense?
* What container sizes should fit underneath the dispenser?
* What should the power source be?
* What type of display or feedback system will be used?
* What method should be used to measure the amount of liquid dispensed?
* What mechanism should be used to control liquid flow?
* What level of dispensing accuracy can the prototype consistently achieve?
* Should Fill-A-Bot detect whether a container is positioned underneath the dispenser before dispensing?
* How should the system detect an empty reservoir or insufficient liquid?
* Which components should be removable to make cleaning and maintenance easier?
