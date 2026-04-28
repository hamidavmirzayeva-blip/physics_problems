# ⚡ Electric Field of Two Point Charges

## 📌 Given
Two charges:
- q at (-a, 0)
- 2q at (a, 0)

Find:
- E(0, y)
- E(x, 0)
- E(x, y)
- Conditions for Ex = 0, Ey = 0, and E = 0
- Numerical value
- Limit y >> a

---

# 🧠 1. General Idea

Electric field from a point charge:

E = k * q / r² (vector direction included)

We resolve components using geometry.

---

# 📍 2. Field at (0, y)

Distance to both charges:
r = √(a² + y²)

### Field from q at (-a, 0)
Direction: from charge to point (0,y)

### Field from 2q at (a, 0)
Same distance, stronger magnitude (2q)

---

### Components

By symmetry:

- x-components do NOT cancel (charges unequal)
- y-components add

Final result:

Ex(0,y) = k * a * q / (a² + y²)^(3/2)

Ey(0,y) = k * y * (3q) / (a² + y²)^(3/2)

---

# 📍 3. Field at (x, 0)

Point lies on x-axis.

Distances:
- to (-a,0): |x + a|
- to (a,0): |x - a|

### Field is purely x-direction:

Ey(x,0) = 0

Ex(x,0) = kq/(x+a)² - k(2q)/(x-a)²

---

# 📍 4. General Field E(x, y)

Let:
r₁ = √((x + a)² + y²)
r₂ = √((x - a)² + y²)

### Vector form:

E = E₁ + E₂

E₁ = kq * (x + a, y) / r₁³  
E₂ = k(2q) * (x - a, y) / r₂³  

So:

Ex = kq(x + a)/r₁³ + 2kq(x - a)/r₂³

Ey = kq(y)/r₁³ + 2kq(y)/r₂³

---

# ⚖️ 5. Conditions

## Ex = 0
Solve:
(x + a)/r₁³ + 2(x - a)/r₂³ = 0

→ no simple symmetry solution (depends on position)

---

## Ey = 0
y factor:

Ey = y * [kq(1/r₁³ + 2/r₂³)]

So:

Ey = 0 when:
- y = 0  (on x-axis)

---

## E = 0 (full cancellation)

Requires:
Ex = 0 AND Ey = 0

From above:
- Ey = 0 ⇒ y = 0
- Then check Ex = 0 on x-axis

So equilibrium lies on x-axis only.

---

# 🔢 6. Numerical Calculation

Given:
a = 0.2 m  
y = 0.3 m  
q = 2 μC = 2 × 10⁻⁶ C  
k = 9 × 10⁹

---

### Step 1: distance
r = √(0.2² + 0.3²)
r = √(0.04 + 0.09)
r = √0.13 ≈ 0.36 m

---

### Step 2: field magnitude scale
kq = 9 × 10⁹ × 2 × 10⁻⁶
kq = 1.8 × 10⁴

---

### Step 3: r³
r³ ≈ (0.36)³ ≈ 0.0467

---

### Step 4: components (order of magnitude)

Ex ≈ (1.8 × 10⁴ × 0.2) / 0.0467  
Ex ≈ 7.7 × 10⁴ N/C

Ey ≈ (1.8 × 10⁴ × 0.3 × 3) / 0.0467  
Ey ≈ 3.5 × 10⁵ N/C

---

# 📊 Final Numerical Result

Ex ≈ 7.7 × 10⁴ N/C  
Ey ≈ 3.5 × 10⁵ N/C  

---

# 🌌 7. Limit y >> a

If y >> a:

r₁ ≈ r₂ ≈ y

So:

Ex → kq( a + 2(-a) ) / y³ = -kqa / y³

Ey → kq(3y) / y³ = 3kq / y²

---

# ✅ Final Insight

- Field becomes mostly vertical (Ey dominant)
- Horizontal component decreases faster
- System behaves like a single effective charge distribution at large distance
