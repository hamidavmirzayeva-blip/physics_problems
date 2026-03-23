# Particle Motion in Time-Dependent Force Field – Notes

## 🔹 Given

- Particle mass: $m = 3 \, \text{kg}$  
- Force as a function of time:

$$
\vec{F}(t) = (15 t, \; 3 t - 12, \; -6 t^2) \, \text{N}
$$

- Initial conditions:  

$$
\vec{r}(0) = (5, 2, -3) \, \text{m}, \quad
\vec{v}(0) = (2, 0, 1) \, \text{m/s}
$$

---

## 🧠 Step 1: Acceleration

Newton’s 2nd law:

$$
\vec{F} = m \vec{a} \quad \Rightarrow \quad \vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

Substitute $m = 3$:

$$
a_x = \frac{15 t}{3} = 5 t
$$

$$
a_y = \frac{3 t - 12}{3} = t - 4
$$

$$
a_z = \frac{-6 t^2}{3} = -2 t^2
$$

✅ Acceleration vector:

$$
\vec{a}(t) = (5 t, \; t - 4, \; -2 t^2) \, \text{m/s}^2
$$

---

## 🧠 Step 2: Velocity

Velocity is the **integral of acceleration**:

$$
\vec{v}(t) = \vec{v}_0 + \int_0^t \vec{a}(t') \, dt'
$$

### X-component:

$$
v_x(t) = 2 + \int_0^t 5 t' \, dt' = 2 + \frac{5 t^2}{2} = 2 + 2.5 t^2
$$

### Y-component:

$$
v_y(t) = 0 + \int_0^t (t' - 4) dt' = \int_0^t t' dt' - \int_0^t 4 dt'
$$

$$
v_y(t) = \frac{t^2}{2} - 4 t
$$

### Z-component:

$$
v_z(t) = 1 + \int_0^t -2 t'^2 dt' = 1 - \frac{2 t^3}{3}
$$

✅ Velocity vector:

$$
\boxed{\vec{v}(t) = \left( 2 + 2.5 t^2, \; \frac{t^2}{2} - 4 t, \; 1 - \frac{2 t^3}{3} \right) \, \text{m/s}}
$$

---

## 🧠 Step 3: Position

Position is the **integral of velocity**:

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(t') dt'
$$

### X-component:

$$
x(t) = 5 + \int_0^t (2 + 2.5 t'^2) dt'
$$

$$
x(t) = 5 + 2 t + \frac{2.5 t^3}{3} = 5 + 2 t + \frac{5}{6} t^3
$$

### Y-component:

$$
y(t) = 2 + \int_0^t \left( \frac{t'^2}{2} - 4 t' \right) dt'
$$

$$
y(t) = 2 + \frac{t^3}{6} - 2 t^2
$$

### Z-component:

$$
z(t) = -3 + \int_0^t \left( 1 - \frac{2 t'^3}{3} \right) dt'
$$

$$
z(t) = -3 + t - \frac{2 t^4}{12} = -3 + t - \frac{t^4}{6}
$$

✅ Position vector:

$$
\boxed{\vec{r}(t) = \left( 5 + 2 t + \frac{5}{6} t^3, \; 2 - 2 t^2 + \frac{t^3}{6}, \; -3 + t - \frac{t^4}{6} \right) \, \text{m}}
$$

---

## 📌 Summary

| Quantity      | Expression |
|---------------|------------|
| **Acceleration** | $\vec{a}(t) = (5 t, \; t - 4, \; -2 t^2)$ m/s² |
| **Velocity**     | $\vec{v}(t) = \left( 2 + 2.5 t^2, \; \frac{t^2}{2} - 4 t, \; 1 - \frac{2 t^3}{3} \right)$ m/s |
| **Position**     | $\vec{r}(t) = \left( 5 + 2 t + \frac{5}{6} t^3, \; 2 - 2 t^2 + \frac{t^3}{6}, \; -3 + t - \frac{t^4}{6} \right)$ m |

---

