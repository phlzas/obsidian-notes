**Derivative of Trigonometric Functions**  

---

## Basic Trigonometric Derivatives:  

| Function         | Derivative                |
|------------------|----------------------------|
| $\sin x$         | $\cos x$                  |
| $\cos x$         | $-\sin x$                 |
| $\tan x$         | $\sec^2 x$                |
| $\cot x$         | $-\csc^2 x$               |
| $\sec x$         | $\sec x \cdot \tan x$     |
| $\csc x$         | $-\csc x \cdot \cot x$    |

---

## Example 1:  
**Function:** $y = \sin x$ at $x = \frac{\pi}{3}$  

### Steps:  
1. **Differentiate:**  
   $$
   \frac{dy}{dx} = \cos x
   $$  

2. **Substitute $x = \frac{\pi}{3}$:**  
   $$
   \frac{dy}{dx} = \cos\left(\frac{\pi}{3}\right) = \frac{1}{2}
   $$  

**Result:**  
$$
\boxed{\frac{1}{2}}
$$  

---

## Example 2:  
**Function:** $y = \sin^3 x$ (i.e., $[\sin x]^3$), at $x = \frac{\pi}{6}$  

### Steps:  
1. **Use Chain Rule:**  
   Let $u = \sin x$  
   $$
   \frac{dy}{dx} = 3(\sin x)^2 \cdot \cos x
   $$  

2. **Substitute $x = \frac{\pi}{6}$:**  
   $$
   \frac{dy}{dx} = 3\left(\frac{1}{2}\right)^2 \cdot \left(\frac{\sqrt{3}}{2}\right) = 3 \cdot \frac{1}{4} \cdot \frac{\sqrt{3}}{2}
   $$  

3. **Simplify:**  
   $$
   \frac{3}{8} \cdot \sqrt{3} = \frac{3\sqrt{3}}{8}
   $$  

**Result:**  
$$
\boxed{\frac{3\sqrt{3}}{8}}
$$  

---

## Key Takeaways:  
- Always **memorize** the basic trigonometric derivatives.  
- Use the **Chain Rule** when trig functions are raised to powers or nested in other functions.  
- Evaluate trig functions at special angles like $\frac{\pi}{6}, \frac{\pi}{3}, \frac{\pi}{4}, \frac{\pi}{2}$ confidently.  

---

## Summary Tip:  
If $y = [\text{Trig}(x)]^n$,  
Then:  
$$
\frac{dy}{dx} = n[\text{Trig}(x)]^{n-1} \cdot \text{Trig}'(x)
$$  
(E.g., $\frac{d}{dx}[\sin^3 x] = 3\sin^2 x \cdot \cos x$)
