# Propagation of Error I

## Given

The radius of the sphere is measured as

$$
r = (6.20 \pm 0.05)\ \text{cm}
$$

We want to calculate:

1. The volume of the sphere
2. The uncertainty in the volume

---

# Step 1: Formula for the Volume of a Sphere

The volume of a sphere is

$$
V = \frac{4}{3}\pi r^3
$$

Substitute the measured radius:

$$
V = \frac{4}{3}\pi (6.20)^3
$$

---

# Step 2: Calculate the Volume

First compute:

$$
(6.20)^3 = 238.328
$$

Then:

$$
V = \frac{4}{3}\pi (238.328)
$$

$$
V \approx 998.3\ \text{cm}^3
$$

---

# Step 3: Propagation of Uncertainty

For a quantity of the form

$$
V \propto r^3
$$

the fractional uncertainty rule gives:

$$
\frac{\Delta V}{V} = 3\frac{\Delta r}{r}
$$

Substitute the values:

$$
\frac{\Delta V}{V}
=
3\left(\frac{0.05}{6.20}\right)
$$

$$
\frac{\Delta V}{V} \approx 0.0242
$$

Now calculate the absolute uncertainty:

$$
\Delta V = V(0.0242)
$$

$$
\Delta V = 998.3 \times 0.0242
$$

$$
\Delta V \approx 24.2\ \text{cm}^3
$$

---

# Final Answer

$$
V = (998 \pm 24)\ \text{cm}^3
$$

---

# Result Summary

| Quantity | Value |
|---|---|
| Radius | $6.20 \pm 0.05\ \text{cm}$ |
| Volume | $998.3\ \text{cm}^3$ |
| Uncertainty in Volume | $\pm 24.2\ \text{cm}^3$ |
| Final Rounded Result | $(998 \pm 24)\ \text{cm}^3$ |
