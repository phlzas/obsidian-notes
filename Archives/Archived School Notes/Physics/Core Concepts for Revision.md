# Core Concepts for Revision  
Related: [[Static Electricity]], [[Dynamic Electricity]], [[Coulomb's Law]], [[Electric Field]], [[Capacitors]], [[Ohm's Law]], [[Resistor Connections]], [[Electromotive Force]], [[Electric Power]]  

---

## Static Electricity  
### Fundamentals  
- **Electric Charge**: Positive (+) and negative (-).  
  - Like charges repel, unlike attract.  
  - Measured in Coulombs (C).  
- **Static Electricity**: Charges at rest, produced by friction.  
  - **Electrostatics**: Study of stationary charges.  
  - **Induction**: Charging without contact (e.g., neutral sphere near charged rod).  

### Coulomb's Law  
$$F = K \frac{q_1 q_2}{d^2}$$  
- $K = 9 \times 10^9\ \text{N·m}^2/\text{C}^2$.  
- **Force**:  
  - Repulsive: Same signs.  
  - Attractive: Opposite signs.  
- **Applications**: Charge interactions, force calculations.  

### Electric Field  
$$E = \frac{F}{q} = \frac{K q}{d^2}$$  
- **Vector Field**:  
  - Lines point from + to -.  
  - Intensity $\propto q$, $\propto \frac{1}{d^2}$.  
- **Uses**: Describes forces on charges, capacitor operation.  

---

## Capacitors  
### Definition  
- Two conductive plates separated by a dielectric.  
- **Capacitance**:  
  $$C = \frac{Q}{V}$$  
  - Stores charge: $Q = C V$.  
  - Energy: $U = \frac{1}{2} C V^2$.  

### Connections  
| Connection | Charge | Voltage | Capacitance |  
|------------|--------|---------|-------------|  
| **Series** | Equal  | Splits  | $\frac{1}{C_{eq}} = \sum \frac{1}{C_i}$ |  
| **Parallel**| Splits | Equal   | $C_{eq} = \sum C_i$ |  

---

## Dynamic Electricity  
### Material Properties  
| Type          | Conductivity ($\sigma$)             | Examples |     |
| ------------- | ----------------------------------- | -------- | --- |
| Conductor     | High ($>10^7\ \text{S/m}$)          | Copper   |     |
| Insulator     | Low ($<10^{-10}\ \text{S/m}$)       | Glass    |     |
| Semiconductor | Medium ($10^{-3}-10^3\ \text{S/m}$) | Silicon  |     |

### Key Quantities  
1. **Current**:  
   $$I = \frac{Q}{t}$$  
   - Conventional: + to -.  
   - Electron: - to +.  

2. **Potential Difference**:  
   $$V = \frac{W}{Q}$$  
   - Measured in Volts (V).  

3. **Resistance**:  
   $$R = \rho \frac{l}{A}$$  
   - $\rho$: Resistivity, $\sigma = \frac{1}{\rho}$: Conductivity.  

---

## Ohm's Law & Circuits  
### Ohm's Law  
$$V = I R$$  
- **Ohmic Materials**: Linear $V-I$ relationship.  
- **Non-Ohmic**: Non-linear.  

### Closed Circuit  
- **EMF**: Total energy per charge.  
- **Ohm's Law**:  
  $$I = \frac{V_B}{R_{eq} + r}$$  
  - $V_B$: EMF, $r$: Internal resistance.  
- **Terminal Voltage**:  
  $$V = V_B - I r$$  

### Resistor Networks  
| Connection | Current | Voltage | Resistance |  
|------------|---------|---------|------------|  
| **Series** | Equal   | Splits  | $R_{eq} = \sum R_i$ |  
| **Parallel**| Splits  | Equal   | $\frac{1}{R_{eq}} = \sum \frac{1}{R_i}$ |  

---

## Electric Power  
$$P = V I = I^2 R = \frac{V^2}{R}$$  
- **Energy**: $E = P t$.  
- **Unit**: Watt (W) = J/s.  
- **Applications**: Heating, lighting, motor operation.  

---

## Critical Constants  
- **Coulomb's Constant**: $K = 9 \times 10^9\ \text{N·m}^2/\text{C}^2$.  
- **Electron Charge**: $e = 1.6 \times 10^{-19}\ \text{C}$.  
- **Copper Resistivity**: $\rho = 1.79 \times 10^{-8}\ \Omega·\text{m}$.  
- **Silver Conductivity**: $\sigma = 6.3 \times 10^7\ \text{S/m}$.  

---

## Problem-Solving Framework  
1. **Classify**: Static or dynamic electricity.  
2. **Identify Connections**: Series, parallel, or mixed.  
3. **Apply Formulas**: Coulomb’s law, Ohm’s law, etc.  
4. **Check Units**: Ensure consistency (e.g., convert μC to C).  
5. **Verify Directions**: Charge polarity, current flow, field lines.  

---

## Practice Problems  
1. Calculate the force between two $10\ \mu\text{C}$ charges 1 m apart.  
2. Find the equivalent resistance of three 5 Ω resistors in parallel.  
3. Determine the terminal voltage of a battery with EMF = 12 V, $r = 0.2\ \Omega$, $R = 4\ \Omega$.  
4. Sketch electric field lines for a +5 μC and -5 μC charge pair.  

[[Formula Sheet]] | [[Electrostatics]] | [[Circuit Analysis]]