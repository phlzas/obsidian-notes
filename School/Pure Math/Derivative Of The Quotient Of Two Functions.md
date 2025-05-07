#PureMath #Study 
**Rule:**  
If $y = \frac{f(x)}{g(x)}$ where $g(x) \neq 0$, then:  
$\frac{dy}{dx} = \frac{g(x) \cdot f'(x) - f(x) \cdot g'(x)}{[g(x)]^2}$  
**Simplified Notation:**  
$\frac{dy}{dx} = \frac{\text{denominator} \cdot (\text{numerator})' - \text{numerator} \cdot (\text{denominator})'}{[\text{denominator}]^2}$

---

## Example 1  
**Function:** $y = \frac{3x - 2}{2x + 3}$ at $x = 1$  

**Solution:**  
$\frac{dy}{dx} = \frac{(2x + 3)(3) - (3x - 2)(2)}{(2x + 3)^2}$  
At $x = 1$:  
$\frac{dy}{dx} = \frac{(2+3)(3) - (3-2)(2)}{(2+3)^2} = \frac{15 - 2}{25} = \boxed{\frac{13}{25}}$  

---

## Example 2  
**Function:** $y = \frac{5x + 11}{x + 2}$ at $x = 0$  

**Solution:**  
$\frac{dy}{dx} = \frac{(x + 2)(5) - (5x + 11)(1)}{(x + 2)^2}$  
At $x = 0$:  
$\frac{dy}{dx} = \frac{(0+2)(5) - (0+11)(1)}{(0+2)^2} = \frac{-1}{4} = \boxed{-\frac{1}{4}}$  

---

## Example 3  
**Function:** $f(x) = \frac{x^2}{3x + 2}$ at $x = -1$  

**Solution:**  
$f'(x) = \frac{(3x + 2)(2x) - x^2(3)}{(3x + 2)^2}$  
At $x = -1$:  
$f'(-1) = \frac{(-3 + 2)(-2) - 1(3)}{(-3 + 2)^2} = \frac{2 - 3}{1} = \boxed{-1}$  

---

## Example 4  
**Angle of Tangent to Curve:** $y = \frac{x - 1}{x^2 - x + 1}$ at $(1, 0)$  

**Solution:**  
$\frac{dy}{dx} = \frac{(x^2 - x + 1)(1) - (x - 1)(2x - 1)}{(x^2 - x + 1)^2}$  
At $x = 1$:  
$\frac{dy}{dx} = \frac{(1 - 1 + 1)(1) - (1 - 1)(2 - 1)}{(1 - 1 + 1)^2} = 1$  
**Angle:**  
$\tan \theta = 1 \quad \Rightarrow \quad \theta = \boxed{45^\circ}$  

---

# Exercise 3 Solutions  

### 1. First Derivative of $y = \frac{2x + 3}{x - 2}$ at $x = 3$  
$\frac{dy}{dx} = \frac{(2)(x - 2) - (2x + 3)(1)}{(x - 2)^2} = \frac{-7}{(x - 2)^2}$  
At $x = 3$:  
$\frac{dy}{dx} \bigg|_{x=3} = \boxed{-7}$  

---

### 2. Slope of Tangent to $y = x - \frac{2}{x}$ at $x = 1$  
$\frac{dy}{dx} = 1 + \frac{2}{x^2}$  
At $x = 1$:  
$\frac{dy}{dx} = 1 + 2 = \boxed{3}$  

---

### 3. Angle with the X-Axis for $y = \frac{1 + x}{1 - x}$ at $(-1, 0)$  
$\frac{dy}{dx} = \frac{2}{(1 - x)^2}$  
At $x = -1$:  
$\frac{dy}{dx} = \frac{2}{4} = 0.5$  
**Angle:**  
$\theta = \arctan(0.5) \approx \boxed{26.6^\circ}$  

---

### 4. Points on $y = \frac{x - 2}{x - 1}$ with Slope = 1  
$\frac{dy}{dx} = \frac{1}{(x - 1)^2} = 1 \implies (x - 1)^2 = 1 \implies x = 0 \text{ or } 2$  
- **At $x = 0$:** $y = \frac{0 - 2}{0 - 1} = \boxed{(0, 2)}$  
- **At $x = 2$:** $y = \frac{2 - 2}{2 - 1} = \boxed{(2, 0)}$  

---

**Key Formulas:**  
- **Quotient Rule:** $\frac{d}{dx}\left(\frac{u}{v}\right) = \frac{u'v - uv'}{v^2}$  
- **Angle Calculation:** $\theta = \arctan(\text{slope})$