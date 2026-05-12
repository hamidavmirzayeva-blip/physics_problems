To calculate the equivalent resistance ($R_{eq}$) of this mixed circuit, we need to break it down section by section, starting from the innermost loops and moving outward.

Since all resistors are $5\ \Omega$, we will use $R = 5\ \Omega$ for each.

---

## 1. Identify Series and Parallel Components

The circuit can be viewed as three main vertical branches connected in parallel, with one additional resistor at the very bottom in parallel with the entire upper structure.

### Step A: The Middle Branch (Series)

The middle vertical branch consists of two resistors in series.


$$\text{Resistance of middle branch } (R_{m}) = R + R = 5 + 5 = 10\ \Omega$$

### Step B: The Right Branch (Series)

The rightmost vertical branch also consists of two resistors in series.


$$\text{Resistance of right branch } (R_{r}) = R + R = 5 + 5 = 10\ \Omega$$

### Step C: The Left Branch (Mixed)

The left section has two resistors in series (top and left-side) which are then in series with the bottom-left resistor. Looking at the nodes:

1. The top and left-most resistors are in series: $5 + 5 = 10\ \Omega$.
2. This $10\ \Omega$ combination is in parallel with the **Middle Branch** ($10\ \Omega$).

---

## 2. Simplifying the Upper Network

Let’s calculate the equivalent resistance of the top-left loop and middle branch combined ($R_{top\_mid}$):


$$\frac{1}{R_{top\_mid}} = \frac{1}{10} + \frac{1}{10}$$

$$R_{top\_mid} = 5\ \Omega$$

Now, this $5\ \Omega$ block is in series with the bottom-left horizontal resistor:


$$R_{left\_side} = 5 + 5 = 10\ \Omega$$

---

## 3. Final Parallel Calculation

We now have three main components remaining between the two primary nodes (the far left and far right junctions):

1. The **Left Side** equivalent: $10\ \Omega$
2. The **Right Branch**: $10\ \Omega$
3. The **Bottom Resistor**: $5\ \Omega$

All three are connected in parallel across the output terminals.

### The Equivalent Resistance ($R_{eq}$):

$$\frac{1}{R_{eq}} = \frac{1}{R_{left\_side}} + \frac{1}{R_{right\_branch}} + \frac{1}{R_{bottom}}$$

Substituting the values:


$$\frac{1}{R_{eq}} = \frac{1}{10} + \frac{1}{10} + \frac{1}{5}$$

$$\frac{1}{R_{eq}} = \frac{1}{10} + \frac{1}{10} + \frac{2}{10}$$

$$\frac{1}{R_{eq}} = \frac{4}{10}$$

---

## Final Result

Solving for $R_{eq}$:


$$R_{eq} = \frac{10}{4} = 2.5\ \Omega$$

> **Summary Table**
> | Section | Calculation | Result |
> | --- | --- | --- |
> | Middle Branch | $5 + 5$ | $10\ \Omega$ |
> | Right Branch | $5 + 5$ | $10\ \Omega$ |
> | Top/Mid Combined | $(10 \parallel 10)$ | $5\ \Omega$ |
> | Total Equivalent | $(10 \parallel 10 \parallel 5)$ | **$2.5\ \Omega$** |
> 
>
