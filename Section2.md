# Section 2: EE Fundamentals

### What is a PCB?

A **PCB** (Printed Circuit Board) is a compact circuit made out of various electrical components and wire traces. In this section of the lab we will explain the different parts that make up a PCB, but firstly we must learn the basics of electricity.

## Introduction to Electricity

Let’s learn how we can mathematically analyze circuits with **Ohm’s law**. Ohm's law relates current, voltage, and resistance in a circuit. Let’s tackle each part of this triangle separately.

![Ohms Law](https://github.com/user-attachments/assets/6206285b-92ac-403f-9860-03dffe5d3d73)

### Current

**Current** is the flow of electricity! More specifically, it is the flow of electrons. We denote the flow of the conventional current opposite the flow of electrons with an arrow on a circuit diagram. The unit of current is amps (A).

### Voltage

But what causes electrons to flow? Power sources contain energy, called **voltage**, creating a difference in potential energy that causes electrons to flow. Picture water flowing downhill, with the hill's height representing voltage. At the top, the water has high potential energy, similar to a high voltage. As the water moves down, it flows naturally to lower points, just like current flows from high voltage to low voltage in a circuit. The steeper the hill (or the greater the voltage difference), the stronger the flow of water, much like a greater voltage difference creates a stronger current. The unit of voltage is voltage (V).

### Resistance

However, the flow of electrons, or current, can be restricted. This is called **resistance**. The unit of resistance is ohms (Ω). Resistance, along with voltage and current are related together by Ohm's law which states V = IR.

Together, using the triangle of Ohm’s law, we can analyze a simple circuit!

### Example

What is the current of this circuit? Note, that the resistor (denoted with the zig-zag line) is what creates resistance in a circuit.

![Ohm's Law Example](https://github.com/user-attachments/assets/08a97061-4578-4e5f-ba22-7a47f4808ac4)

## Components and Nodal Analysis

**Components** are a part that makes up an electrical circuit. Now we will discuss a variety of common components and how to use them:

### Power Supply

First, we need a **power source**. A power source is something that has voltage and thus powers the circuit itself. Here is a wide range of power sources you might have to work with, but for this lab the **direct current (DC)** power supply will be used.

![Power Symbols](https://github.com/user-attachments/assets/82e676c1-cb27-4912-be61-d7c9323fe407)

### Resistors

Next, we have the **resistor** we just saw before. These add resistance to the circuit. We add resistance to control the flow of current and the levels of voltage around the circuit. Controlling current and voltage is especially important for adjusting levels of signals and preventing problems like shorts which will be discussed later.

When calculating the total resistance across a path of wire with multiple resistors using Ohm’s law, we need to learn how to calculate resistors in series or in parallel. Here are pictures of both concepts, each with the method of calculation. 

![Resistors in Series and Parallel](https://github.com/user-attachments/assets/e34f8b16-ee6d-4a5d-af94-dcd6ba0adcc0)

### Voltage Divider Example

With these two components we can construct a common circuit element called a voltage divider, which can be used to explain a few more concepts.

![Voltage Divider](https://github.com/user-attachments/assets/52e14943-2c3a-401b-a43e-191a8f2327d4)

A resistor can divide two different voltages, as we think of wires as ideal conductors with zero resistance. Each conductive wire that connects two or more components together is called a node and each node has a given voltage! Each node is color coded in the picture. When we calculate the voltage and current in a circuit, we are measuring these values at certain nodes. To aid in calculating voltage and current at certain nodes, we can use **Kirchhoff’s Laws**.

### Kirchhoff's Laws

![Kirchhoff's Laws](https://github.com/user-attachments/assets/903ad1e2-ed55-463e-9411-91b1f4364417)

Kirchhoff’s Current Law (KCL) states that the amount of current entering a node is equal to the amount exiting the node. Kirchhoff's Voltage Law (KVL) states that the sum of voltage around a loop is zero. Think of these as a form of conservation of energy.

With this we can calculate the voltage at each node using KVL:

![KVL Problem](https://github.com/user-attachments/assets/06eacd0f-be9d-4eb1-918d-a8631d08f7ab)

The triangle symbol attached to the green node at the bottom represents ground. Ground is defined as a place on a circuit with no voltage. 

For future reference, we can calculate a voltage divider with this equation:

![Voltage Divider Rule](https://github.com/user-attachments/assets/d84b608d-3dd2-4cd9-8d5e-779f0e671e2f)

### Power

You may also have to deal with power in a circuit. This is calculated with this equation:

![Electric Power](https://github.com/user-attachments/assets/ea7f302d-5b70-48b1-bb71-4fc8c105e4a2)

This idea of power explains why a **short circuit** is so dangerous. A short is where there is some low resistance path that bypasses resistance in a circuit. As seen, a conductor connecting a very high potential and low potential node will create a massive amount of power. If the conductor inherently has some low resistance value like 0.0005, the power going through the light will change from some manageable value to wattage in the hundred thousands. We should be careful of shorts as they can break components and destroy our circuits. 

![Short Circuit](https://github.com/user-attachments/assets/37458df0-a9cd-43a9-b9d0-2b81b3857697)

Another important concept is an open circuit, which is caused by a break in the circuit. This mathematically can be represented as the circuit at the break having infinite resistance. By Ohm’s law, an open circuit must have zero current flow which will cause the circuit to no longer work.

![Open Circuit](https://github.com/user-attachments/assets/5eb74d1b-1add-4eb4-bdb1-511036a08e0b)
