# Propagation of Error II

## Given

The dimensions of the rectangular plate are:

$$
L = (15.3 \pm 0.1)\ \text{cm}
$$

$$
W = (8.4 \pm 0.1)\ \text{cm}
$$

We want to calculate:

1. The area of the plate
2. The uncertainty in the area

---

# Step 1: Formula for Area

The area of a rectangle is

$$
A = LW
$$

Substitute the measured values:

$$
A = (15.3)(8.4)
$$

---

# Step 2: Calculate the Area

$$
A = 128.52\ \text{cm}^2
$$

---

# Step 3: Propagation of Uncertainty

For multiplication, fractional uncertainties add:

$$
\frac{\Delta A}{A}
=
\frac{\Delta L}{L}
+
\frac{\Delta W}{W}
$$

Substitute the values:

$$
\frac{\Delta A}{A}
=
\frac{0.1}{15.3}
+
\frac{0.1}{8.4}
$$

$$
\frac{\Delta A}{A}
=
0.00654 + 0.01190
$$

$$
\frac{\Delta A}{A}
\approx 0.01844
$$

Now calculate the absolute uncertainty:

$$
\Delta A = A(0.01844)
$$

$$
\Delta A = 128.52 \times 0.01844
$$

$$
\Delta A \approx 2.37\ \text{cm}^2
$$

---

# Final Answer

$$
A = (128.5 \pm 2.4)\ \text{cm}^2
$$

---

# Result Summary

| Quantity | Value |
|---|---|
| Length | $15.3 \pm 0.1\ \text{cm}$ |
| Width | $8.4 \pm 0.1\ \text{cm}$ |
| Area | $128.52\ \text{cm}^2$ |
| Uncertainty in Area | $\pm 2.37\ \text{cm}^2$ |
| Final Rounded Result | $(128.5 \pm 2.4)\ \text{cm}^2$ |
