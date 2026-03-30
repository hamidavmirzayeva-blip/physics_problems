# Damped Harmonic Oscillator

---

## Equation of Motion

The motion of a damped harmonic oscillator is described by:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + kx = 0
$$

where:  
- $m$ = mass  
- $b$ = damping coefficient  
- $k$ = spring constant  
- $x(t)$ = displacement  

---

## Characteristic Equation

Assume a solution of the form $x(t) = e^{rt}$:

$$
m r^2 + b r + k = 0
$$

Solve using the quadratic formula:

$$
r = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

---

## Key Parameters

Define:

$$
\omega_0 = \sqrt{\frac{k}{m}} \quad \text{(natural frequency)}
$$

$$
\gamma = \frac{b}{2m} \quad \text{(damping factor)}
$$

---

## Classification of Motion

The behavior depends on the discriminant:

$$
b^2 - 4mk
$$

---

### 🟢 Underdamped Case ($b^2 < 4mk$)

- Oscillatory motion with exponential decay  

$$
x(t) = e^{-\gamma t} \left( C_1 \cos(\omega_d t) + C_2 \sin(\omega_d t) \right)
$$

where:

$$
\omega_d = \sqrt{\omega_0^2 - \gamma^2}
$$

---

### 🟡 Critically Damped Case ($b^2 = 4mk$)

- Fastest return to equilibrium without oscillation  

$$
x(t) = (C_1 + C_2 t)e^{-\gamma t}
$$

---

### 🔴 Overdamped Case ($b^2 > 4mk$)

- No oscillations, slow return to equilibrium  

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

where:

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

---

## Numerical Solution (RK4 Method)

Convert to a system of first-order equations:

Let:

$$
x' = v
$$

$$
v' = \frac{-b v - k x}{m}
$$

---

### RK4 Update Equations

At each time step:

$$
k_1^x = v, \quad k_1^v = a(x,v)
$$

$$
k_2^x = v + \frac{dt}{2}k_1^v, \quad k_2^v = a\left(x + \frac{dt}{2}k_1^x, v + \frac{dt}{2}k_1^v\right)
$$

$$
k_3^x = v + \frac{dt}{2}k_2^v, \quad k_3^v = a\left(x + \frac{dt}{2}k_2^x, v + \frac{dt}{2}k_2^v\right)
$$

$$
k_4^x = v + dt \cdot k_3^v, \quad k_4^v = a(x + dt \cdot k_3^x, v + dt \cdot k_3^v)
$$

Update:

$$
x_{n+1} = x_n + \frac{dt}{6}(k_1^x + 2k_2^x + 2k_3^x + k_4^x)
$$

$$
v_{n+1} = v_n + \frac{dt}{6}(k_1^v + 2k_2^v + 2k_3^v + k_4^v)
$$

---

## Effect of Damping Coefficient $b$

- Small $b$ → oscillations (underdamped)  
- $b = 2\sqrt{mk}$ → fastest return (critical)  
- Large $b$ → slow, no oscillation (overdamped)  

---

## Graphs

### Position vs Time
- Underdamped → oscillating decay  
- Critical → fastest drop to zero  
- Overdamped → slow decay  

### Phase Portrait $(x, v)$
- Underdamped → spiral into origin  
- Critical → straight approach  
- Overdamped → curved non-oscillatory path  

---

## Summary

| Case | Condition | Behavior |
|------|----------|---------|
| Underdamped | $b^2 < 4mk$ | Oscillatory decay |
| Critical | $b^2 = 4mk$ | Fastest non-oscillatory |
| Overdamped | $b^2 > 4mk$ | Slow non-oscillatory |

> **Key Insight:** The damping coefficient $b$ controls whether the system oscillates and how quickly it returns to equilibrium.
