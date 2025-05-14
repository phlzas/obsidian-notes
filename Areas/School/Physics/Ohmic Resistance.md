# Ohmic Resistance  
Related: [[Ohm's Law]], [[Resistivity]], [[Conductivity]]  

---

## Key Concepts  
### Electric Resistance  
- **Definition**: Opposition to current flow due to friction.  
- **Formula**:  
  $$R = \rho_e \frac{l}{A}$$  
  - $R$: Resistance (Ω).  
  - $\rho_e$: Resistivity (Ω·m).  
  - $l$: Length (m).  
  - $A$: Cross-sectional area (m²).  

### Resistivity ($\rho_e$)  
- **Definition**: Resistance of a 1 m long, 1 m² cross-section conductor.  
- **Unit**: Ohm-meter (Ω·m).  
- **Property**: Material-specific, temperature-dependent.  

### Conductivity ($\sigma_e$)  
- **Definition**: Reciprocal of resistivity.  
- **Formula**:  
  $$\sigma_e = \frac{1}{\rho_e}$$  
- **Unit**: $\Omega^{-1}\ \text{m}^{-1}$ (Siemens/m).  

---

## Solved Problems  
1. **Current in Copper Wire**:  
   - $l = 30\ \text{m}$, $A = 2 \times 10^{-6}\ \text{m}^2$, $V = 3\ \text{V}$, $\rho_e = 1.79 \times 10^{-8}\ \Omega·\text{m}$.  
   - Solution:  
     $$R = \frac{\rho_e l}{A} = \frac{(1.79 \times 10^{-8})(30)}{2 \times 10^{-6}} = 0.2685\ \Omega$$  
     $$I = \frac{V}{R} = \frac{3}{0.2685} \approx 11.17\ \text{A}$$  

2. **Conductivity of Wire**:  
   - $l = 1\ \text{m}$, $A = 1\ \text{mm}^2 = 10^{-6}\ \text{m}^2$, $I = 4\ \text{A}$, $V = 2\ \text{V}$.  
   - Solution:  
     $$R = \frac{V}{I} = \frac{2}{4} = 0.5\ \Omega$$  
     $$R = \rho_e \frac{l}{A} \implies 0.5 = \rho_e \frac{1}{10^{-6}} \implies \rho_e = 5 \times 10^{-7}\ \Omega·\text{m}$$  
     $$\sigma_e = \frac{1}{\rho_e} = \frac{1}{5 \times 10^{-7}} = 2 \times 10^6\ \Omega^{-1}\ \text{m}^{-1}$$  

---

**Practice Questions**:  
1. Calculate the resistance of a 2 m copper wire with $A = 1\ \text{mm}^2$.  
2. Find the conductivity of a material with $\rho_e = 2 \times 10^{-7}\ \Omega·\text{m}$.  
3. Explain how increasing wire length affects resistance.  

[[Ohm's Law]] | [[Resistor Connections]] | [[Dynamic Electricity]]