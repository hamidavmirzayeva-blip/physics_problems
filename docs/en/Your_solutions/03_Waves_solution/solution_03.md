# Standing Wave from Two Traveling Waves

We are given two waves:

$$
y_1(x,t) = A \sin(kx - \omega t)
$$

$$
y_2(x,t) = A \sin(kx + \omega t)
$$

---

## Step 1: Resulting wave by superposition

The **resulting wave** is the sum:

$$
y(x,t) = y_1 + y_2 = A \sin(kx - \omega t) + A \sin(kx + \omega t)
$$

Using the trigonometric identity:

$$
\sin \alpha + \sin \beta = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)
$$

Let $\alpha = kx - \omega t$, $\beta = kx + \omega t$:

$$
y(x,t) = 2 A \sin\left(\frac{(kx - \omega t) + (kx + \omega t)}{2}\right) 
           \cos\left(\frac{(kx - \omega t) - (kx + \omega t)}{2}\right)
$$

Simplify:

$$
y(x,t) = 2 A \sin(kx) \cos(\omega t)
$$

✅ This is the **standing wave equation**.

---

## Step 2: Node positions

Nodes occur where the amplitude is **always zero**, i.e.,

$$
\sin(kx) = 0
$$

So:

$$
kx = n \pi, \quad n = 0, 1, 2, \dots
$$

or

$$
x_n = \frac{n \pi}{k}
$$

These are the positions of the **nodes**.

---

## Step 3: Antinodes

Antinodes occur where the amplitude is maximum:

$$
\sin(kx) = \pm 1 \implies kx = \frac{\pi}{2} + n \pi
$$

or

$$
x_\text{antinode} = \frac{\pi}{2k} + \frac{n \pi}{k}, \quad n = 0, 1, 2, \dots
$$
