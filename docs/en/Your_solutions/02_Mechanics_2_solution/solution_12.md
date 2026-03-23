# Motion under Constant Force – Notes

## 🔹 Given

- Mass: $m = 2 \, \text{kg}$  
- Constant force: $\vec{F} = [6, 2] \, \text{N}$  
- Initial velocity: $\vec{v}_0 = [1, -1] \, \text{m/s}$  
- Initial position: $\vec{r}_0 = [0, 0] \, \text{m}$  

---

## 🧠 Step 1: Acceleration

Newton's 2nd law:

$$
\vec{a} = \frac{\vec{F}}{m}
$$

$$
a_x = \frac{6}{2} = 3 \, \text{m/s}^2
$$

$$
a_y = \frac{2}{2} = 1 \, \text{m/s}^2
$$

✅ Acceleration vector:

$$
\boxed{\vec{a}(t) = [3, 1] \, \text{m/s}^2}
$$

---

## 🧠 Step 2: Velocity

Integrate acceleration:

$$
\vec{v}(t) = \vec{v}_0 + \vec{a} t
$$

$$
v_x(t) = 1 + 3 t
$$

$$
v_y(t) = -1 + 1 t = t - 1
$$

✅ Velocity vector:

$$
\boxed{\vec{v}(t) = [1 + 3t, t - 1] \, \text{m/s}}
$$

---

## 🧠 Step 3: Position

Integrate velocity:

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(t') dt'
$$

### X-component:

$$
x(t) = \int_0^t (1 + 3 t') dt' = t + \frac{3 t^2}{2}
$$

### Y-component:

$$
y(t) = \int_0^t (t' - 1) dt' = \frac{t^2}{2} - t
$$

✅ Position vector:

$$
\boxed{\vec{r}(t) = \left[t + \frac{3}{2} t^2, \; \frac{t^2}{2} - t \right] \, \text{m}}
$$

---

## 🧠 Step 4: Trajectory

Eliminate $t$:

$$
x = t + \frac{3}{2} t^2 \quad \Rightarrow \quad t = ? 
$$

- This is quadratic; for plotting, it's easier to **plot parametric curve**: $(x(t), y(t))$.


plt.xlabel('x [m]')
plt.ylabel('y [m]')
plt.title('Trajectory of particle under constant force')
plt.grid(True)
plt.show()
