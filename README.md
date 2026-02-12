# Siemens-PLC-Conveyor-Station
"Automated Material Sorting System using Siemens S7-1200 &amp; TIA Portal V18. Features HSC positioning, HMI control, and structured State Machine logic."

# Automated Material Sorting Conveyor System 🏭

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Platform](https://img.shields.io/badge/Platform-Siemens_TIA_Portal_V18-blue)

## 📖 Introduction
This project is part of the Automation Laboratory coursework at SeAMK. It focuses on developing a robust control system for a conveyor belt to sort materials based on specific logic using **Siemens S7-1200 PLC** and **KTP700 Basic HMI**.

Unlike traditional timer-based approaches, this system utilizes **High-Speed Counters (HSC)** for precise positioning, ensuring accuracy regardless of mechanical speed variations.

---

#
## ⚙️ Key Features
* [cite_start]**Precise Positioning:** Implemented HSC (High-Speed Counter) logic to track workpiece location on the belt with millimeter accuracy[cite: 317].
* **Structured Modes:**
    * [cite_start]**Auto Mode:** Continuous sorting logic based on user input (Short Press = Sort to Bin 1, Long Press = Sort to Bin 2)[cite: 318, 319].
    * [cite_start]**Manual Mode:** Full manual control via HMI for maintenance and testing[cite: 295].
    * [cite_start]**Reference Run:** Automatic homing sequence to clear the belt and reset sensors before operation[cite: 301].
* [cite_start]**Safety Interlocks:** Logic prevents belt movement if pneumatic cylinders are extended to avoid mechanical damage[cite: 297].
* **HMI Interface:** User-friendly dashboard for monitoring sensor states, mode switching, and alarm history.

## 🛠️ Technology Stack
* **PLC:** Siemens S7-1200 CPU
* **HMI:** Siemens KTP700 Basic
* **Software:** TIA Portal V18
* **Languages:** Ladder Diagram (LAD), Function Block Diagram (FBD)
* **Actuators:** DC Motor (Conveyor), Pneumatic Cylinders (Sorting)

## 📂 Project Structure
* `/Conveyor Station`: Contains the archived TIA Portal project file (`.ap18`).
* `/Docs`: Technical documentation and I/O lists.
* `/HMI Screen`: Images of the HMI screens and logic segments.

## 🚀 How to Run
1.  Open **TIA Portal V18**.
2.  Retrieve the archived project file from the `Conveyor Station` folder.
3.  Extract the "FB_library_AE23_IEPIP24.7z" and put it in the same folder with the `Conveyor Station` folder.
4.  Load the program into PLCSIM or physical S7-1200 hardware.
5.  Connect the HMI simulation.

---
*Created by Minh Nhat Nguyen - Automation Engineering Student @ SeAMK*
