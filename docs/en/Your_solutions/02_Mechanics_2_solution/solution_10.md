# Particle Motion in 3D Force Field – Notes

## 🔹 Given

Particle mass: $m = 0.5 \, \text{kg}$  

Position as a function of time:

$$
x(t) = 5 t^2 - t
$$

$$
y(t) = 2 t^3
$$

$$
z(t) = -3 t + 2
$$

---

## 🧠 Step 1: Velocity

Velocity is the **time derivative** of position:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \left(\frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt}\right)
$$

Compute each component:

$$
v_x = \frac{dx}{dt} = 10 t - 1
$$

$$
v_y = \frac{dy}{dt} = 6 t^2
$$

$$
v_z = \frac{dz}{dt} = -3
$$

✅ Velocity vector:

$$
\boxed{\vec{v}(t) = (10t - 1)\hat{i} + 6 t^2 \hat{j} - 3 \hat{k} \, \text{m/s}}
$$

---

## 🧠 Step 2: Momentum

Momentum:

$$
\vec{p}(t) = m \vec{v}(t)
$$

Substitute $m = 0.5$:

$$
p_x = 0.5 (10t - 1) = 5 t - 0.5
$$

$$
p_y = 0.5 \cdot 6 t^2 = 3 t^2
$$

$$
p_z = 0.5 \cdot (-3) = -1.5
$$

✅ Momentum vector:

$$
\boxed{\vec{p}(t) = (5 t - 0.5)\hat{i} + 3 t^2 \hat{j} - 1.5 \hat{k} \, \text{kg·m/s}}
$$

---

## 🧠 Step 3: Acceleration

Acceleration is the **derivative of velocity**:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \left(\frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt}\right)
$$

Compute each component:

$$
a_x = \frac{d}{dt}(10t - 1) = 10
$$

$$
a_y = \frac{d}{dt}(6 t^2) = 12 t
$$

$$
a_z = \frac{d}{dt}(-3) = 0
$$

✅ Acceleration vector:

$$
\boxed{\vec{a}(t) = 10\hat{i} + 12 t \hat{j} + 0 \hat{k} \, \text{m/s}^2}
$$

---

## 🧠 Step 4: Force

Newton’s 2nd law:

$$
\vec{F}(t) = m \vec{a}(t)
$$

$$
F_x = 0.5 \cdot 10 = 5
$$

$$
F_y = 0.5 \cdot 12 t = 6 t
$$

$$
F_z = 0.5 \cdot 0 = 0
$$

✅ Force vector:

$$
\boxed{\vec{F}(t) = 5 \hat{i} + 6 t \hat{j} + 0 \hat{k} \, \text{N}}
$$

---

## 🧠 Step 5: Power

Instantaneous power transferred by the field:

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t)
$$

Compute dot product:

$$
P(t) = F_x v_x + F_y v_y + F_z v_z
$$

Substitute:

$$
P(t) = 5 (10t - 1) + (6 t)(6 t^2) + 0(-3)
$$

$$
P(t) = 50 t - 5 + 36 t^3
$$

$$
P(t) = 36 t^3 + 50 t - 5 \, \text{W}
$$

✅ Power as a function of time:

$$
\boxed{P(t) = 36 t^3 + 50 t - 5 \, \text{W}}
$$

---

## 📌 Summary

| Quantity      | Expression |
|---------------|------------|
| **Velocity**  | $\vec{v}(t) = (10t-1)\hat{i} + 6 t^2 \hat{j} - 3 \hat{k}$ m/s |
| **Momentum**  | $\vec{p}(t) = (5t-0.5)\hat{i} + 3 t^2 \hat{j} - 1.5 \hat{k}$ kg·m/s |
| **Acceleration** | $\vec{a}(t) = 10\hat{i} + 12 t \hat{j} + 0 \hat{k}$ m/s² |
| **Force**     | $\vec{F}(t) = 5\hat{i} + 6 t \hat{j} + 0 \hat{k}$ N |
| **Power**     | $P(t) = 36 t^3 + 50 t - 5$ W |
