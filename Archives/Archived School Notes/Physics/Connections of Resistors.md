# Connections of Resistors  
Related: [[Ohm's Law]], [[Electric Resistance]], [[Dynamic Electricity]]  

---

## Key Concepts  
### Series Connection  
- **Properties**:  
  - Same current: $I = I_1 = I_2 = I_3$.  
  - Voltage splits: $V_t = V_1 + V_2 + V_3$.  
  - Equivalent resistance:  
    $$R_{eq} = R_1 + R_2 + R_3$$  
  - For $N$ equal resistors ($R$): $R_{eq} = N R$.  
- **Note**: Higher resistance increases voltage drop ($V \propto R$).  

### Parallel Connection  
- **Properties**:  
  - Same voltage: $V = V_1 = V_2 = V_3$.  
  - Current splits: $I_t = I_1 + I_2 + I_3$.  
  - Equivalent resistance:  
    $$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$  
  - For $N$ equal resistors ($R$): $R_{eq} = \frac{R}{N}$.  
- **Note**: Higher resistance reduces current ($I \propto \frac{1}{R}$).  

---

## Solved Problems  
1. **Series Circuit**:  
   - $V = 45\ \text{V}$, $R_1 = 5\ \Omega$, $R_2 = 10\ \Omega$.  
   - a) $R_{eq} = 5 + 10 = 15\ \Omega$.  
   - b) $I = \frac{V}{R_{eq}} = \frac{45}{15} = 3\ \text{A}$.  
   - c) $V_1 = I R_1 = 3 \times 5 = 15\ \text{V}$, $V_2 = 3 \times 10 = 30\ \text{V}$.  

2. **Parallel Circuit**:  
   - $R_1 = 60\ \Omega$, $R_2 = 30\ \Omega$, $R_3 = 20\ \Omega$, $V = 90\ \text{V}$.  
   - a) $\frac{1}{R_{eq}} = \frac{1}{60} + \frac{1}{30} + \frac{1}{20} \implies R_{eq} = 10\ \Omega$.  
   - b) $I_t = \frac{V}{R_{eq}} = \frac{90}{10} = 9\ \text{A}$.  
   - c) $I_1 = \frac{90}{60} = 1.5\ \text{A}$, $I_2 = \frac{90}{30} = 3\ \text{A}$, $I_3 = \frac{90}{20} = 4.5\ \text{A}$.  

3. **Mixed Circuit**:  
   - $5\ \Omega$ and $1\ \Omega$ in series: $R = 5 + 1 = 6\ \Omega$.  
   - $6\ \Omega$ and $3\ \Omega$ in parallel: $R_{eq} = \frac{6 \times 3}{6 + 3} = 2\ \Omega$.  
   - Total current: $I_t = \frac{V}{R_{eq}} = \frac{4}{2} = 2\ \text{A}$.  
   - Current through $1\ \Omega$:  
     $$I_1 \times 6 = 2 \times 2 \implies I_1 = \frac{4}{6} \approx 0.667\ \text{A}$$  

---

**Practice Questions**:  
1. Find $R_{eq}$ for three 10 Ω resistors in parallel.  
2. Calculate the voltage drop across a 4 Ω resistor in series with a 6 Ω resistor, total $V = 20\ \text{V}$.  
3. Explain why parallel resistors have lower equivalent resistance.  

[[Ohm's Law]] | [[Electric Power]] | [[Dynamic Electricity]]