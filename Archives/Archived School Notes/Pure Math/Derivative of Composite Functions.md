**Derivative of Composite Functions**   

**Chain Rule:**  
If $y = [f(x)]^n$, then:  
$$
\frac{dy}{dx} = n[f(x)]^{n-1} \cdot f'(x)
$$  

---

## Example 1:  
**Function:** $y = (x^3 + 3x^2 - 1)^7$ at $x = 0$.  

### Steps:  
1. **Identify the outer and inner functions:**  
   - Outer: $u^7$, where $u = x^3 + 3x^2 - 1$.  
   - Inner: $u = x^3 + 3x^2 - 1$.  

2. **Differentiate outer and inner functions:**  
   - $\frac{dy}{du} = 7u^6$.  
   - $\frac{du}{dx} = 3x^2 + 6x$.  

3. **Apply the chain rule:**  
   $$
   \frac{dy}{dx} = 7(x^3 + 3x^2 - 1)^6 \cdot (3x^2 + 6x)
   $$  

4. **Substitute $x = 0$:**  
   $$
   \frac{dy}{dx} = 7(0 + 0 - 1)^6 \cdot (0 + 0) = 0
   $$  

**Result:**  
$$
\boxed{0}
$$  

---

## Example 2:  
**Function:** $y = z^3$, where $z = 2x^2 - 3x + 1$, at $x = 2$.  

### Steps:  
1. **Express $y$ in terms of $x$:**  
   $$
   y = (2x^2 - 3x + 1)^3
   $$  

2. **Differentiate outer and inner functions:**  
   - Outer: $u^3$, where $u = 2x^2 - 3x + 1$.  
   - $\frac{dy}{du} = 3u^2$.  
   - $\frac{du}{dx} = 4x - 3$.  

3. **Apply the chain rule:**  
   $$
   \frac{dy}{dx} = 3(2x^2 - 3x + 1)^2 \cdot (4x - 3)
   $$  

4. **Substitute $x = 2$:**  
   $$
   \frac{dy}{dx} = 3(8 - 6 + 1)^2 \cdot (8 - 3) = 3(3)^2 \cdot 5 = 135
   $$  

**Result:**  
$$
\boxed{135}
$$  

---

## Key Takeaways:  
- **Simplified Rule:**  
  $$
  \frac{d}{dx}[f(x)^n] = n \cdot f(x)^{n-1} \cdot f'(x)
  $$  

- **Critical Steps:**  
  1. Identify the outer and inner functions.  
  2. Differentiate the outer function *with respect to the inner function*.  
  3. Multiply by the derivative of the inner function.  

- **Common Mistakes:**  
  - Forgetting to multiply by the derivative of the inner function.  
  - Mishandling exponents (e.g., not reducing the power by 1).  
  - Arithmetic errors when substituting values.  
