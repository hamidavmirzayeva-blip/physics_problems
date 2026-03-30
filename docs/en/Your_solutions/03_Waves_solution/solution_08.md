# Traveling Wave Function Check

We are asked which of the following functions can describe a **traveling wave**.  
We use the **1D wave equation**:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

A function satisfies this equation if it can describe a traveling wave.

---

## Given Functions

1. $y(x,t) = A \cos(k x^2 - \omega t)$  
2. $y(x,t) = A (x - v t)^2$  
3. $y(x,t) = A \log(x + v t)$  

---

## Step 1: Option (a)

$$
y(x,t) = A \cos(k x^2 - \omega t)
$$

- Second derivatives:  

$$
\frac{\partial^2 y}{\partial x^2} \neq \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}
$$

- **Reason:** The $x$-dependent term in $\partial^2 y / \partial x^2$ makes it not proportional to $\partial^2 y / \partial t^2$.  

❌ **Option (a) does NOT satisfy the wave equation.**

---

## Step 2: Option (b)

$$
y(x,t) = A (x - vt)^2
$$

- Second derivatives:  

$$
\frac{\partial^2 y}{\partial x^2} = 2A, \quad \frac{\partial^2 y}{\partial t^2} = 2Av^2
$$

- Check wave equation:  

$$
\frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = \frac{2Av^2}{v^2} = 2A = \frac{\partial^2 y}{\partial x^2}
$$

✅ **Option (b) satisfies the wave equation.**

---

## Step 3: Option (c)

$$
y(x,t) = A \log(x + v t)
$$

- Second derivatives:  

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}, \quad \frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}
$$

- Check wave equation:  

$$
\frac{1}{v^2} \frac{\partial^2 y}{\partial t^2} = -\frac{A}{(x+vt)^2} = \frac{\partial^2 y}{\partial x^2}
$$

✅ **Option (c) satisfies the wave equation.**

---

## ✅ Conclusion

| Option | Function | Satisfies Wave Equation? | Can Be a Traveling Wave? |
|--------|---------|------------------------|-------------------------|
| (a)    | $A \cos(k x^2 - \omega t)$ | ❌ No | ❌ |
| (b)    | $A (x - v t)^2$             | ✅ Yes | ✅ |
| (c)    | $A \log(x + v t)$           | ✅ Yes | ✅ |
