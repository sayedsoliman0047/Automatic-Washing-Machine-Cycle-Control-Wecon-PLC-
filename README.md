#  Automatic Washing Machine Cycle Control (Wecon PLC)

##  Project Overview

This project simulates an **automatic washing machine cycle** using a Wecon PLC, implemented and tested on a real hardware control board.

The system controls a motor in two directions (**Forward and Reverse**) with timed delays, creating a continuous washing cycle similar to real industrial or home washing machines.

The process runs automatically in a loop until the stop command is pressed.

---

##  Technology Stack

* PLC: Wecon PLC
* Programming Software: Wecon PLC Software
* Control Type: Sequential Cyclic Control
* Hardware: Real Control Board (Contactors, Timers, Relays)

---

##  System Workflow

The system operates in a continuous cycle:

1. Press **Start**
2. Motor runs **Forward (KF)** for 5 seconds
3. Motor stops for 2 seconds
4. Motor runs **Reverse (KR)** for 5 seconds
5. Motor stops for 2 seconds
6. Cycle repeats automatically:

 Forward → Stop → Reverse → Stop → Repeat

 Press **Stop** → System stops immediately

---

##  Control Logic Explanation

* The system is based on **sequential cyclic logic**
* Two contactors are used:

  * Forward Contactor (KF)
  * Reverse Contactor (KR)
* Timers are used to:

  * Control motor running time (5 seconds)
  * Create delay between direction changes (2 seconds)
* Interlocking logic ensures:

  * Forward and Reverse cannot run at the same time
* The system behaves like a **looped state machine**

---

##  Technical Highlights

* Bidirectional Motor Control (Forward / Reverse)
* Time-Based Sequential Operation
* Continuous Loop Automation
* Electrical Interlocking for Safety
* Real Hardware Implementation
* Industrial Control Concept Simulation

---

##  Project Implementation

* Designed using Wecon PLC programming software
* Logic tested and verified
* Implemented on a real electrical board
* Contactors used for direction control
* Timers configured for precise operation

---

##  How to Run

1. Power ON the system
2. Press **Start**
3. Observe automatic cycle:

   * Forward → Stop → Reverse → Stop
4. System continues automatically
5. Press **Stop** to terminate operation

---

##  Future Improvements

* Add adjustable timing using HMI
* Integrate water level and load sensors
* Add fault protection system
* Implement speed control using VFD

---

##  Demo

[Watch The Project](video.mp4)

---

##  Files Included

* PLC Program File (Wecon)
* Demo Video (Real Operation)

---

##  Notes

This project demonstrates:

* Understanding of cyclic control systems
* Motor direction control techniques
* Timer-based automation logic
* Real-world industrial control implementation

---
