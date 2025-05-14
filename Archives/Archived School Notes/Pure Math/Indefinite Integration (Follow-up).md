**Indefinite Integration (Follow-up)**  

---

### Example 1:  
$$
\int \frac{1}{x} dx = \ln |x| + C
$$  

---

### Example 2:  
$$
\int x \cdot \cos x dx
$$  

Use **Integration by Parts**:  
Let:  
- $u = x \Rightarrow du = dx$  
- $dv = \cos x dx \Rightarrow v = \sin x$  

Then:  
$$
\int x \cos x dx = x \sin x - \int \sin x dx = x \sin x + \cos x + C
$$  

**Result:**  
$$
\boxed{x \sin x + \cos x + C}
$$  

---

### Example 3:  
$$
\int \frac{2x}{x^2 + 1} dx
$$  

Let $u = x^2 + 1 \Rightarrow du = 2x dx$  

Then:  
$$
\int \frac{2x}{x^2 + 1} dx = \int \frac{du}{u} = \ln|u| + C = \ln(x^2 + 1) + C
$$  

**Result:**  
$$
\boxed{\ln(x^2 + 1) + C}
$$  

---

### Tip:  
- Use substitution when you see a function and its derivative in the same integral.  
- Use parts when the product of two functions is present.
