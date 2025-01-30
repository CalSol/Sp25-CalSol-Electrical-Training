# Section 2: EE Fundamentals

### What is a PCB?

A **PCB** (Printed Circuit Board) is a compact circuit made out of various electrical components and wire traces. In this section of the lab we will explain the different parts that make up a PCB, but firstly we must learn the basics of electricity.

### Introduction to Electricity

Let’s learn how we can mathematically analyze circuits with **Ohm’s law**. Ohm's law relates current, voltage, and resistance in a circuit. Let’s tackle each part of this triangle separately.

![Ohms Law](https://github.com/user-attachments/assets/6206285b-92ac-403f-9860-03dffe5d3d73)

**Current** is the flow of electricity! More specifically, it is the flow of electrons. We denote the flow of the conventional current opposite the flow of electrons with an arrow on a circuit diagram. The unit of current is amps (A).

But what causes electrons to flow? Power sources contain energy, called **voltage**, creating a difference in potential energy that causes electrons to flow. Picture water flowing downhill, with the hill's height representing voltage. At the top, the water has high potential energy, similar to a high voltage. As the water moves down, it flows naturally to lower points, just like current flows from high voltage to low voltage in a circuit. The steeper the hill (or the greater the voltage difference), the stronger the flow of water, much like a greater voltage difference creates a stronger current. The unit of voltage is voltage (V).

However, the flow of electrons, or current, can be restricted. This is called **resistance**. The unit of resistance is ohms (Ω).

Together, using the triangle of Ohm’s law, we can analyze a simple circuit!

### Example

What is the current of this circuit? Note, that the resistor (denoted with the zig-zag line) is what creates resistance in a circuit.

![Ohm's Law Example](https://github.com/user-attachments/assets/08a97061-4578-4e5f-ba22-7a47f4808ac4)

## Components and Nodal Analysis

**Components** are a part that makes up an electrical circuit. Now we will discuss a variety of common components and how to use them:

First, we need a **power source**. A power source is something that has voltage and thus powers the circuit itself. Here is a wide range of power sources you might have to work with, but for this lab the **direct current (DC)** power supply will be used.

![Power Symbols](https://github.com/user-attachments/assets/82e676c1-cb27-4912-be61-d7c9323fe407)

Next, we have the **resistor** we just saw before. These add resistance to the circuit. We add resistance to control the flow of current and the levels of voltage around the circuit. Controlling current and voltage is especially important for adjusting levels of signals and preventing problems like shorts which will be discussed later.

When calculating the total resistance across a path of wire with multiple resistors using Ohm’s law, we need to learn how to calculate resistors in series or in parallel. Here are pictures of both concepts, each with the method of calculation. 

![Resistors in Series and Parallel](https://github.com/user-attachments/assets/e34f8b16-ee6d-4a5d-af94-dcd6ba0adcc0)

With these two components we can construct a common circuit element called a voltage divider, which can be used to explain a few more concepts.

![Voltage Divider](https://github.com/user-attachments/assets/52e14943-2c3a-401b-a43e-191a8f2327d4)

A resistor can divide two different voltages, as we think of wires as ideal conductors with zero resistance. Each conductive wire that connects two or more components together is called a node and each node has a given voltage! Each node is color coded in the picture. When we calculate the voltage and current in a circuit, we are measuring these values at certain nodes. To aid in calculating voltage and current at certain nodes, we can use **Kirchhoff’s Laws**.

![Kirchhoff's Laws](https://github.com/user-attachments/assets/903ad1e2-ed55-463e-9411-91b1f4364417)

