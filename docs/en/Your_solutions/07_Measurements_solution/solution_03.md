# Propagation of Error III

## Given

Voltage:

$$
V = (10.0 \pm 0.2)\ \text{V}
$$

Current:

$$
I = (2.00 \pm 0.05)\ \text{A}
$$

We want to find:

1. Resistance
2. Uncertainty in resistance

---

# Step 1: Ohm’s Law

Resistance is given by:

$$
R = \frac{V}{I}
$$

Substitute values:

$$
R = \frac{10.0}{2.00}
$$

---

# Step 2: Calculate Resistance

$$
R = 5.00\ \Omega
$$

---

# Step 3: Propagation of Uncertainty

For division, fractional uncertainties add:

$$
\frac{\Delta R}{R} = \frac{\Delta V}{V} + \frac{\Delta I}{I}
$$

Substitute values:

$$
\frac{\Delta R}{R}
=
\frac{0.2}{10.0} + \frac{0.05}{2.00}
$$

$$
\frac{\Delta R}{R}
=
0.02 + 0.025
$$

$$
\frac{\Delta R}{R} = 0.045
$$

---

# Step 4: Absolute Uncertainty

$$
\Delta R = R \cdot 0.045
$$

$$
\Delta R = 5.00 \times 0.045
$$

$$
\Delta R = 0.225\ \Omega
$$

---

# Final Answer

$$
R = (5.00 \pm 0.23)\ \Omega
$$

---

# Result Summary

| Quantity | Value |
|---|---|
| Voltage | $10.0 \pm 0.2\ \text{V}$ |
| Current | $2.00 \pm 0.05\ \text{A}$ |
| Resistance | $5.00\ \Omega$ |
| Uncertainty | $\pm 0.23\ \Omega$ |
| Final Result | $(5.00 \pm 0.23)\ \Omega$ |
