A projectile is fired from the ground with an initial velocity of 
100
 m/s
 at an angle of 
37
∘
 above the horizontal. Assume no air resistance.

Derive the differential equations of motion in the horizontal and vertical directions.

Determine the time of flight.

Determine the maximum height.

Determine the range.

# 1. What is projectile motion?

Projectile motion is when an object is **thrown into the air at an angle** and moves under **gravity only**.

Example: throwing a ball.

The motion has **two independent parts**:

* **Horizontal motion (x direction)**
* **Vertical motion (y direction)**

---

# 2. Given in the problem

Initial velocity
v₀ = 100 m/s

Angle
θ = 37°

Gravity
g = 9.8 m/s²

---

# 3. Split the velocity

We split the initial velocity into **horizontal** and **vertical** components.

Horizontal velocity:

vₓ = v₀ cosθ

Vertical velocity:

vᵧ = v₀ sinθ

Using approximations:

sin(37°) ≈ 0.6
cos(37°) ≈ 0.8

So:

vₓ = 100 × 0.8 = **80 m/s**

vᵧ = 100 × 0.6 = **60 m/s**

---

# 4. Differential equations of motion

## Horizontal direction

There is **no force horizontally**, so acceleration is **0**.

Second derivative of position:

d²x/dt² = 0

Integrate once:

dx/dt = vₓ = constant

Integrate again:

x(t) = vₓ t

Since vₓ = 80:

x(t) = **80t**

---

## Vertical direction

Gravity acts downward.

d²y/dt² = −g

So:

d²y/dt² = −9.8

Integrate:

dy/dt = vᵧ − gt

Integrate again:

y(t) = vᵧ t − (1/2)gt²

Substitute vᵧ = 60:

y(t) = **60t − 4.9t²**
This equation tells us how high the projectile is at time t.
---

# 5. Time of flight

Time of flight = how long the projectile stays in the air

Formula:

T = (2 v₀ sinθ) / g

Substitute values:

T = (2 × 100 × 0.6) / 9.8

T = 120 / 9.8

T ≈ **12.2 s**

---

# 6. Maximum height

Formula:

H = (v₀² sin²θ) / (2g)

Substitute values:

H = (100² × 0.6²) / (2 × 9.8)

H = (10000 × 0.36) / 19.6

H = 3600 / 19.6

H ≈ **184 m**

So the projectile goes about 184 meters high.
---

# 7. Range

Range = how far the projectile travels horizontally.

Formula:

R = (v₀² sin(2θ)) / g

Since:

sin(74°) ≈ 0.96

R = (100² × 0.96) / 9.8

R = 9600 / 9.8

R ≈ **980 m**

Meaning the projectile lands about 980 meters away.
---

# Final answers

Differential equations:

Horizontal
d²x/dt² = 0

Vertical
d²y/dt² = −g

Time of flight ≈ **12.2 s**

Maximum height ≈ **184 m**

Range ≈ **980 m**


