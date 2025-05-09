# 🔢 Digital Two-Digit Counter

A sequential logic system built to function as a two-digit **digital counter**. This project demonstrates how counting logic is implemented using integrated circuits, displayed through seven-segment displays, and constructed both virtually and physically.

---

## 🏫 Project Information

* **University:** Benha University, Faculty of Engineering (Shoubra)  
* **Department:** Communications and Computer Engineering  
* **Course:** Logic Design / Digital Circuits  

---

## 👩‍💻 Team Members

* Farida Waheed Abdelbary  
* Mohamed Ahmed Mohamed Hassan  
* Abdelrahman Salah El-dein Abdelaziz  
* Raneem Ahmed Refaat  
* Razan Ahmed Fawzy  

---

## 📌 Project Overview

The system is designed to:

* Count from 00 to 99 and reset
* Use IC-based logic to perform binary counting
* Display output on **dual seven-segment displays**
* Demonstrate clock-driven incrementing
* Be simulated in **Proteus** and implemented on **breadboard & PCB**

---

## 🧠 System Features

* **Synchronous counting** up to 99
* **IC 74LS90**: Decade counter for each digit
* **IC 7447**: BCD to 7-segment decoder
* **Clock pulse** drives incrementation
* **Reset control** to reinitialize count

---

## ⚙️ Components & Connections

| Component            | Quantity | Description                                      |
|----------------------|----------|--------------------------------------------------|
| **74LS90**           | 2        | Decade counter (divide-by-10)                   |
| **7447**             | 2        | BCD to 7-segment decoder                        |
| **7-Segment Display**| 2        | Common anode type                               |
| **Clock Generator**  | 1        | Generates pulses to increment counter           |
| **Resistors**        | 14       | Current limiting for 7-segment display          |
| **Push Button**      | 1        | Manual reset input                              |
| **Capacitors**       | 2        | Debouncing or delay stabilization               |
| **Breadboard / PCB** | 1 each   | For simulation and real implementation          |

---

## 🧾 How It Works

1. A **clock pulse** is generated and fed into the first **74LS90**, which counts 0–9.
2. Once the first digit reaches 9 and rolls over, it triggers the **second 74LS90**.
3. The **7447 decoders** convert the BCD output into signals that light up the correct segments of each display.
4. The **push button** can reset the entire system to 00.

---

## 📐 Design Steps

1. **Proteus Schematic**:
   - Design using ICs and simulated seven-segment displays.
   - Add a clock source and reset.
2. **PCB Layout**:
   - Convert schematic into board layout in Proteus.
3. **Breadboard Prototype**:
   - Test live wiring with real ICs and components.
4. **Final PCB Product**:
   - Solder all components and validate real-world functionality.

---

## 🧪 Testing Results

| Test Scenario             | Expected Behavior             | Passed |
|---------------------------|-------------------------------|--------|
| Counter increments        | From 00 to 99                 | ✅     |
| Reset function            | Counter returns to 00         | ✅     |
| Clock pulse propagation   | Correct carry to 2nd digit    | ✅     |
| Display decoding accuracy | Correct digit illumination    | ✅     |

---

## 💾 Project Files

* `Digital Counter.pdf` – Report with design, circuit images, and implementation
* `Proteus Design` – Includes schematic and PCB layout (to be added manually)

---

## 🖼 Circuit Design

* **Simulation**: Full design simulated on Proteus  
* **Implementation**:
  - Breadboard-tested
  - Final build completed on custom PCB board

---

## 📷 Screenshots

* Proteus schematic and PCB layout

  ![image](https://github.com/user-attachments/assets/14305bda-5e74-48b5-9396-3750c79d3463)
* Breadboard implementation photo

  ![image](https://github.com/user-attachments/assets/cef8aab7-73f3-4bf7-aba6-f9fbd18d3c8f)
* Real PCB final product

  ![image](https://github.com/user-attachments/assets/de7c4e64-6b9b-4bc9-acb4-6d32a0d949ff)

---

## 🛠 Tools Used

* **Proteus** – Circuit simulation and PCB design  
* **Multimeter** – Continuity and voltage verification  
* **Soldering Kit** – PCB assembly  
* **Common Lab Components** – Passive elements and logic ICs  
