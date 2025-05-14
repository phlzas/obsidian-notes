# The Electric Capacitor  
Related: [[Static Electricity]], [[Electric Field]], [[Dynamic Electricity]]  

---

## Key Concepts  
### Capacitor  
- **Definition**: Two parallel metal plates separated by an insulator (dielectric).  
- **Function**: Stores charge, creates potential difference.  
- **Formula**:  
  $$C = \frac{Q}{V}$$  
  - $C$: Capacitance (Farads, F).  
  - $Q$: Charge on one plate (C).  
  - $V$: Potential difference (V).  

### Charging Process  
- **Connection to Battery**:  
  - Plate A (positive pole) gains positive charge.  
  - Plate B (negative pole) gains negative charge.  
  - Charge transfer stops when $V_{\text{capacitor}} = V_{\text{battery}}$.  
- **Charge Relation**:  
  $$Q = C V$$  

### Capacitor Connections  
| Connection | Charge | Voltage | Capacitance Formula |  
|------------|--------|---------|---------------------|  
| **Series** | Equal ($Q = Q_1 = Q_2$) | Splits ($V_t = V_1 + V_2$) | $\frac{1}{C_{eq}} = \sum \frac{1}{C_i}$ |  
| **Parallel**| Splits ($Q_t = Q_1 + Q_2$) | Equal ($V_t = V_1 = V_2$) | $C_{eq} = \sum C_i$ |  

---

## Solved Problem  
- **Given**: Network with capacitors (12 μF, 6 μF in series; 3 μF, 11 μF, and series result in parallel; 9 μF in series with parallel result).  
- **Find**: Equivalent capacitance.  
- **Solution**:  
  - Series (12 μF, 6 μF):  
    $$\frac{1}{C'} = \frac{1}{12} + \frac{1}{6} \implies C' = 4\ \mu\text{F}$$  
  - Parallel (3 μF, 11 μF, 4 μF):  
    $$C'' = 3 + 11 + 4 = 18\ \mu\text{F}$$  
  - Series (18 μF, 9 μF):  
    $$\frac{1}{C_{eq}} = \frac{1}{18} + \frac{1}{9} \implies C_{eq} = 6\ \mu\text{F}$$  

---

**Practice Questions**:  
1. Calculate the charge on a 10 μF capacitor with 5 V across it.  
2. Derive the equivalent capacitance for three 4 μF capacitors in series.  
3. Explain why capacitors in parallel have the same voltage.  

[[Electric Field]] | [[Dynamic Electricity]] | [[Electrostatics]]