**Derivative of Trigonometric Functions (Follow-up)**  

---

## More Complex Examples:  

### Example 1:  
**Function:** $y = \tan x + \sec x$ at $x = \frac{\pi}{4}$  

**Steps:**  
1. **Differentiate:**  
   $$
   \frac{dy}{dx} = \sec^2 x + \sec x \cdot \tan x
   $$  

2. **Substitute $x = \frac{\pi}{4}$:**  
   $$
   \sec\left(\frac{\pi}{4}\right) = \sqrt{2}, \quad \tan\left(\frac{\pi}{4}\right) = 1  
   $$  
   $$
   \frac{dy}{dx} = (\sqrt{2})^2 + \sqrt{2} \cdot 1 = 2 + \sqrt{2}
   $$  

**Result:**  
$$
\boxed{2 + \sqrt{2}}
$$  

---

### Example 2:  
**Function:** $y = \frac{\cos x}{\sin x}$ (i.e., $\cot x$)  

**Differentiate using quotient rule:**  
Let $y = \frac{u}{v}$ where $u = \cos x$, $v = \sin x$  
Then:  
$$
\frac{dy}{dx} = \frac{v \cdot u' - u \cdot v'}{v^2} = \frac{\sin x \cdot (-\sin x) - \cos x \cdot \cos x}{\sin^2 x}
$$  
$$
= \frac{-\sin^2 x - \cos^2 x}{\sin^2 x} = \frac{-1}{\sin^2 x} = -\csc^2 x
$$  

**Result:**  
$$
\boxed{-\csc^2 x}
$$  

---

## Tips:  
- Be comfortable using quotient rule and chain rule for trigonometric expressions.  
- Simplify your expressions **before** substituting values to avoid errors.  
