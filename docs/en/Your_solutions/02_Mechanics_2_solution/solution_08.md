# One-Dimensional Harmonic Force – Notes

## 🔹 Given

- Force:

$$
F(x) = -kx
$$

where $k$ is a positive constant (spring constant).

---

## 🧠 Step 1: Equation of Motion

Newton's 2nd law:

$$
F = m a = m \frac{d^2 x}{dt^2}
$$

Substitute $F(x)$:

$$
m \frac{d^2 x}{dt^2} = - k x
$$

Rewriting:

$$
\frac{d^2 x}{dt^2} + \frac{k}{m} x = 0
$$

This is the **simple harmonic oscillator equation**.

---

## 🔸 Step 2: Solve the Equation

The general solution:

$$
x(t) = A \cos(\omega t) + B \sin(\omega t)
$$

where

$$
\omega = \sqrt{\frac{k}{m}}
$$

$A$ and $B$ are constants determined by initial conditions.  

- If $x(0) = x_0$ and $v(0) = 0$:

$$
x(t) = x_0 \cos(\omega t)
$$

---

## 🧠 Step 3: Work Done from $0$ to $x_0$

Work done by a force:

$$
W = \int_{0}^{x_0} F(x) \, dx
$$

Substitute $F(x) = -kx$:

$$
W = \int_0^{x_0} (-kx) \, dx
$$

$$
W = -k \int_0^{x_0} x \, dx
$$

$$
W = -k \left[ \frac{x^2}{2} \right]_0^{x_0}
$$

$$
W = -\frac{1}{2} k x_0^2
$$

**Interpretation:** The work done **by the force is negative** (it opposes displacement).  

- The **potential energy** stored in the spring is:

$$
U(x_0) = \frac{1}{2} k x_0^2
$$

- So:

$$
F(x) = - \frac{dU}{dx} = - \frac{d}{dx} \left( \frac{1}{2} k x^2 \right) = - k x
$$

✅ This verifies the relationship.

---

## 🔹 Step 4: Graphs

- Force vs position:

$$
F(x) = - k x
$$

- Potential energy vs position:

$$
U(x) = \frac{1}{2} k x^2
$$

### Sketch Description:

- $F(x)$: straight line through origin with negative slope (-k).  
- $U(x)$: parabola opening upwards, minimum at $x = 0$.

---

## 📌 Summary

- **Equation of motion:**  

$$
\frac{d^2 x}{dt^2} + \frac{k}{m} x = 0
$$

- **Solution:**  

$$
x(t) = x_0 \cos\left(\sqrt{\frac{k}{m}} \, t\right)
$$

- **Work / Potential Energy:**  

$$
U(x) = \frac{1}{2} k x^2, \quad F = - \frac{dU}{dx}
$$

- **Graphs:**  
  - $F(x)$: linear negative slope  
  - $U(x)$: parabola
