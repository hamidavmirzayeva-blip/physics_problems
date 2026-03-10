### **1. What does “area under a curve” mean?**

* Imagine you draw the graph of a function, like **f(x) = sin(x)**.
* The **area under the curve** is the space between the curve and the x-axis, from **x = 0** to **x = π**.
* To find this area, we use **integration**.

Think of integration as **adding up tiny slices** of the graph to get the total area.

---

### **2. How to calculate it step by step**

#### Step 2.1: Write the integral

For a function f(x) from x = a to x = b:

```
Area = ∫ from a to b of f(x) dx
```

Here:

```
f(x) = sin(x)
a = 0
b = π
```

So we write:

```
Area = ∫ from 0 to π of sin(x) dx
```

---

#### Step 2.2: Find the antiderivative

* The antiderivative is the **opposite of taking the derivative**.
* We know: the derivative of cos(x) is −sin(x).
* That means the antiderivative of sin(x) is:

```
∫ sin(x) dx = −cos(x)
```

---

#### Step 2.3: Apply the limits (from 0 to π)

* Definite integral formula:

```
∫[0 to π] sin(x) dx = [−cos(x)] from 0 to π
```

* This means: plug in the top limit, then subtract the bottom limit:

```
= (−cos(π)) − (−cos(0))
```

* cos(π) = −1, so −cos(π) = 1
* cos(0) = 1, so −cos(0) = −1

```
= 1 − (−1) = 1 + 1 = 2
```

---

### ✅ **Answer:**

```
Area = 2
```
