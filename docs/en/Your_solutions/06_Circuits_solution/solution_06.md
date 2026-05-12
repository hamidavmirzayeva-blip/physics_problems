To find the current flowing through the ammeter, we will use **Kirchhoff’s Laws**. The ammeter is located in the left branch of the circuit. Let's define our currents and loops.

---

## 1. Define Currents (KCL)

At the top-left node:

* $I_A$: Current through the ammeter (left branch).
* $I_1$: Current through the right branch ($R_1$).
* $I_2$: Current through the middle branch ($R_2$).

By **Kirchhoff's Current Law (KCL)**:


$$I_A = I_1 + I_2 \quad \text{(Eq. 1)}$$

---

## 2. Apply Voltage Laws (KVL)

### Loop 1 (Top Loop - Clockwise)

Starting from the node above the ammeter:


$$\mathcal{E}_2 - I_2 R_2 - I_A r_w = 0$$


Substitute values ($\mathcal{E}_2 = 4.5\text{V}$, $R_2 = 20\,\Omega$, $r_w = 1\,\Omega$):


$$4.5 - 20I_2 - 1I_A = 0 \implies I_A + 20I_2 = 4.5 \quad \text{(Eq. 2)}$$

### Loop 2 (Outer Loop - Clockwise)

Starting from the node above the ammeter and going through the outermost path:


$$\mathcal{E}_2 - I_1 R_1 - I_1 r_w + \mathcal{E}_1 - I_A r_w = 0$$


Substitute values ($\mathcal{E}_2 = 4.5\text{V}$, $\mathcal{E}_1 = 9\text{V}$, $R_1 = 10\,\Omega$, $r_w = 1\,\Omega$):


$$4.5 - 10I_1 - 1I_1 + 9 - 1I_A = 0$$

$$13.5 - 11I_1 - I_A = 0 \implies I_A + 11I_1 = 13.5 \quad \text{(Eq. 3)}$$

---

## 3. Solve the System

From **Eq. 1**, we know $I_1 = I_A - I_2$. Substitute this into **Eq. 3**:


$$I_A + 11(I_A - I_2) = 13.5$$

$$12I_A - 11I_2 = 13.5 \quad \text{(Eq. 4)}$$

Now we have a system with **Eq. 2** and **Eq. 4**:

1. $I_A + 20I_2 = 4.5 \implies I_2 = \frac{4.5 - I_A}{20}$
2. $12I_A - 11I_2 = 13.5$

Substitute $I_2$ into Eq. 4:


$$12I_A - 11\left(\frac{4.5 - I_A}{20}\right) = 13.5$$


Multiply everything by 20 to clear the fraction:


$$240I_A - 11(4.5 - I_A) = 270$$

$$240I_A - 49.5 + 11I_A = 270$$

$$251I_A = 319.5$$

---

## Final Result

$$I_A = \frac{319.5}{251} \approx 1.273\ \text{A}$$

The current flowing through the ammeter is approximately **$1.27\ \text{A}$**.
