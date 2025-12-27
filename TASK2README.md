# **Task 2 – 4-bit Ripple Carry Adder (Verilog)**

## **Objective**

To design and simulate a multi-bit digital component using hierarchical modeling in Verilog. This task demonstrates how a complex circuit can be built using simpler building blocks.

---

## **Description**

In this task, a **4-bit Ripple Carry Adder (RCA)** is designed using four instances of a **1-bit Full Adder** (developed in Task-1). The carry output of each full adder is connected to the carry input of the next adder, allowing multi-bit addition.

The design is simulated using **EDA Playground** to verify correct sum and carry propagation for various 4-bit input combinations.

---

## **Design Details**

### **Modules Used**

* **full_adder**
  Performs single-bit addition with carry-in and carry-out.
* **rca_4bit**
  A 4-bit ripple carry adder constructed using four full adder modules.

### **Inputs**

* `A[3:0]` – 4-bit input operand
* `B[3:0]` – 4-bit input operand
* `Cin` – Carry input

### **Outputs**

* `Sum[3:0]` – 4-bit sum output
* `Cout` – Final carry output

---

## **Testbench**

A Verilog testbench was written to validate the design using real binary values.

### **Test Cases**

| A (Decimal) | B (Decimal) | Expected Sum |
| ----------- | ----------- | ------------ |
| 5           | 3           | 8            |
| 9           | 6           | 15           |
| 15          | 1           | 16           |
| 7           | 8           | 15           |

Each test case was simulated with appropriate time delays, and the simulation completed successfully.

---

## **Simulation Tool**

* **EDA Playground**
* Simulator: **Icarus Verilog**
* Language: **Verilog / SystemVerilog**
* Simulation Link: https://www.edaplayground.com/x/QviZ

---

## **Results**

* The design compiled without errors.
* All test cases produced correct sum and carry outputs.
* The ripple carry mechanism was verified through simulation.

---

## **Learning Outcomes**

* Understanding hierarchical design in Verilog
* Working with multi-bit buses
* Reusing modules to build larger digital systems
* Writing and simulating a structured testbench

---

## **Files Included**

* `design.sv` – Contains the `full_adder` and `rca_4bit` modules
* `testbench.sv` – Testbench for validating the 4-bit ripple carry adder
The 4-bit Ripple Carry Adder was successfully designed and simulated using hierarchical modeling. This task strengthens the understanding of modular design and multi-bit arithmetic circuits in digital systems.

