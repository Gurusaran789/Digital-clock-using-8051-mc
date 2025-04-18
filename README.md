

Digital Clock Using 8051 Microcontroller
Project Overview

This project is a **Digital Clock** developed using the **8051 microcontroller**. The primary objective is to display the current time on a 7-segment display or an LCD. The clock uses a simple real-time clock circuit to keep track of time accurately.
Features
- Displays time in HH:MM:SS format.
- Uses a **8051 microcontroller** for control and processing.
- Simulated and tested using **Keil** (IDE) and **Proteus** (for simulation).
- Optionally supports **adjustment of time** using external switches or buttons.

Components Used
- 8051 Microcontroller** (AT89C51 or equivalent)
- **7-segment display** or **LCD** (16x2)
- **Crystal Oscillator** (for clock generation)
- **Resistors, Capacitors, Diodes**
- **Push buttons** (optional for setting time)

## **Working Principle**

The **8051 microcontroller** operates the digital clock, generating the required signals to drive the display. It uses **timer interrupts** to increment the seconds and then update the minute and hour counters accordingly. The microcontroller drives the 7-segment display or LCD to display the time in a 24-hour format.

### **How It Works**
- **Timer Interrupt**: The **8051 timer** is configured to generate an interrupt every 1 second.
- **Time Calculation**: Each interrupt increments the second counter. Once the seconds reach 60, the minute counter is incremented, and similarly for the hour.
- **Display**: The time is displayed on a **7-segment display** or **LCD**. If using a 7-segment display, multiple displays are used to show hours, minutes, and seconds.

## **Software Used**
- **Keil uVision**: For writing and compiling the C code for the 8051 microcontroller.
- **Proteus**: For simulating the circuit and testing the functionality of the project before hardware implementation.

## **Installation & Setup**

1. Clone the repository or download the files from the GitHub link.
2. Open the project in **Keil** to compile the C code for the **8051** microcontroller.
3. Use **Proteus** to simulate the project and ensure proper operation.
4. Connect the 7-segment display or LCD to the appropriate pins on the **8051** microcontroller as per the circuit diagram.

## **Code Explanation**
- **Main Program**: Contains the logic for initializing the system, setting up the timer interrupt, and updating the display.
- **Interrupt Service Routine**: Handles the timer interrupt to increment the second, minute, and hour counters.
- **Display Control**: Manages the logic to drive the 7-segment display or LCD to show the current time.

## **Conclusion**

This project successfully demonstrates a **Digital Clock** using an **8051 microcontroller**. It serves as a great learning tool for understanding embedded systems, microcontrollers, and real-time clock operations.

## **License**

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

-
