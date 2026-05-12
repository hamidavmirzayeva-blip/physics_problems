To solve for the currents $I_1$, $I_2$, and $I_3$, we apply **Kirchhoff's Current Law (KCL)** and **Kirchhoff's Voltage Law (KVL)**.

---

## 1. Define Currents and Directions

Let's define the currents at the top junction (node):

* $I_1$: Current in the left branch (flowing right).
* $I_2$: Current in the middle branch (flowing down through $R_2$).
* $I_3$: Current in the right branch (flowing left from $E_2$).

According to **KCL** at the top node:


$$I_1 + I_3 = I_2 \implies I_1 - I_2 + I_3 = 0 \quad \text{(Eq. 1)}$$

---

## 2. Apply Kirchhoff’s Voltage Law (KVL)

### Loop 1 (Left Loop - Clockwise)

Starting from the bottom-left corner and moving clockwise:


$$-I_1 R_1 - I_2 R_2 + \mathcal{E}_1 - I_1 r_w = 0$$


Substitute the values ($R_1=20$, $R_2=10$, $r_w=1$, $\mathcal{E}_1=4.5$):


$$-20I_1 - 10I_2 + 4.5 - 1I_1 = 0$$

$$-21I_1 - 10I_2 = -4.5 \implies 21I_1 + 10I_2 = 4.5 \quad \text{(Eq. 2)}$$

### Loop 2 (Right Loop - Counter-Clockwise)

Starting from the bottom-right and moving counter-clockwise through the middle:


$$\mathcal{E}_2 - I_3 r_w - I_2 R_2 = 0$$


Substitute the values ($\mathcal{E}_2=9$, $r_w=1$, $R_2=10$):


$$9 - 1I_3 - 10I_2 = 0 \implies 10I_2 + I_3 = 9 \quad \text{(Eq. 3)}$$

---

## 3. Solve the System of Equations

From **Eq. 3**, express $I_3$ in terms of $I_2$:


$$I_3 = 9 - 10I_2$$

Substitute $I_3$ into **Eq. 1**:


$$I_1 - I_2 + (9 - 10I_2) = 0$$

$$I_1 - 11I_2 = -9 \implies I_1 = 11I_2 - 9$$

Now substitute this expression for $I_1$ into **Eq. 2**:


$$21(11I_2 - 9) + 10I_2 = 4.5$$

$$231I_2 - 189 + 10I_2 = 4.5$$

$$241I_2 = 193.5$$

$$I_2 = \frac{193.5}{241} \approx 0.803\ \text{A}$$

### Find $I_1$ and $I_3$:

$$I_1 = 11(0.803) - 9 \approx -0.167\ \text{A}$$


*(The negative sign means the actual current $I_1$ flows in the opposite direction assigned).*

$$I_3 = 9 - 10(0.803) \approx 0.970\ \text{A}$$

---

## Final Results

| Current | Value (Amperes) |
| --- | --- |
| $I_1$ | $-0.167\ \text{A}$ |
| $I_2$ | $0.803\ \text{A}$ |
| $I_3$ | $0.970\ \text{A}$ |
