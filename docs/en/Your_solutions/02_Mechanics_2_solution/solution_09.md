# Motion with Linear Drag – Notes

## 🔹 Given

Equation of motion:

$$
m \frac{dv}{dt} = -mg - k v
$$

- Initial conditions:  
  $v(0) = v_0$, $x(0) = 10$  
- $m$ = mass, $g$ = gravity, $k$ = linear drag coefficient  

---

## 🧠 Step 1: Rewrite the equation

Divide both sides by $m$:

$$
\frac{dv}{dt} = -g - \frac{k}{m} v
$$

Let:

$$
\alpha = \frac{k}{m}
$$

Then:

$$
\frac{dv}{dt} + \alpha v = -g
$$

This is a **first-order linear ODE**.

---

## 🔸 Step 2: Solve for $v(t)$ (analytical solution)

The integrating factor is:

$$
\mu(t) = e^{\int \alpha dt} = e^{\alpha t}
$$

Multiply both sides:

$$
e^{\alpha t} \frac{dv}{dt} + \alpha e^{\alpha t} v = - g e^{\alpha t}
$$

Left-hand side is derivative:

$$
\frac{d}{dt} \left( v e^{\alpha t} \right) = - g e^{\alpha t}
$$

Integrate both sides:

$$
v e^{\alpha t} = - \frac{g}{\alpha} e^{\alpha t} + C
$$

$$
v(t) = - \frac{g}{\alpha} + C e^{-\alpha t}
$$

Use initial condition $v(0) = v_0$:

$$
v_0 = - \frac{g}{\alpha} + C
$$

$$
C = v_0 + \frac{g}{\alpha}
$$

✅ So the solution:

$$
\boxed{v(t) = -\frac{g}{\alpha} + \left(v_0 + \frac{g}{\alpha} \right) e^{-\alpha t}}
$$

---

## 🧠 Step 3: Solve for $x(t)$

$$
x(t) = x_0 + \int_0^t v(t') dt'
$$

$$
x(t) = x_0 + \int_0^t \left[ -\frac{g}{\alpha} + \left(v_0 + \frac{g}{\alpha} \right) e^{-\alpha t'} \right] dt'
$$

Integrate:

$$
x(t) = x_0 - \frac{g}{\alpha} t + \left(v_0 + \frac{g}{\alpha} \right) \frac{1 - e^{-\alpha t}}{\alpha}
$$

✅ Analytical solution:

$$
\boxed{x(t) = x_0 + \frac{v_0 + g/\alpha}{\alpha} (1 - e^{-\alpha t}) - \frac{g}{\alpha} t}
$$

---

## 🔹 Step 4: Maximum Height

Maximum height occurs when $v(t_\text{max}) = 0$:

$$
0 = -\frac{g}{\alpha} + \left(v_0 + \frac{g}{\alpha} \right) e^{-\alpha t_\text{max}}
$$

Solve for $t_\text{max}$:

$$
e^{-\alpha t_\text{max}} = \frac{g/\alpha}{v_0 + g/\alpha}
$$

$$
t_\text{max} = -\frac{1}{\alpha} \ln \left( \frac{g/\alpha}{v_0 + g/\alpha} \right)
$$

Then plug $t_\text{max}$ into $x(t)$ to find **maximum height**.

---

## 🔹 Step 5: Compare with no drag

Without drag ($k = 0$):

- $v(t) = v_0 - g t$  
- $x(t) = x_0 + v_0 t - \frac{1}{2} g t^2$  

Maximum height:

$$
x_\text{max} = x_0 + \frac{v_0^2}{2 g}
$$

- With drag: maximum height is **lower** due to energy loss.

---

## 🔹 Step 6: Numerical Simulation

