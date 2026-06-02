# Geostationary Orbit

---

## 1. Condition for Geostationary Orbit

A satellite is geostationary if it stays above the same point on Earth.

This requires its orbital period to match Earth’s rotation period:

$$
T = 24\ \text{hours}
$$

More precisely:

$$
T = 23.93\ \text{hours} = 86164\ \text{s}
$$

(This is one sidereal day, not 24 h solar day.)

---

## 2. Formula for Orbital Radius

For circular orbit:

$$
T = 2\pi \sqrt{\frac{r^3}{GM}}
$$

Rearranging:

$$
r^3 = \frac{GMT^2}{4\pi^2}
$$

---

## 3. Given Values

Gravitational constant:

$$
G = 6.67 \times 10^{-11}
$$

Earth mass:

$$
M = 5.97 \times 10^{24}\ \text{kg}
$$

Period:

$$
T = 86164\ \text{s}
$$

---

## 4. Compute Orbital Radius

First compute:

$$
GM \approx 3.986 \times 10^{14}
$$

Substitute:

$$
r^3 = \frac{(3.986 \times 10^{14})(86164)^2}{4\pi^2}
$$

This gives:

$$
r \approx 4.216 \times 10^{7}\ \text{m}
$$

Convert to km:

$$
r \approx 42164\ \text{km}
$$

---

## 5. Altitude Above Earth’s Surface

Earth radius:

$$
R = 6378\ \text{km}
$$

Altitude:

$$
h = r - R
$$

$$
h = 42164 - 6378
$$

$$
h \approx 35786\ \text{km}
$$

---

## 6. Final Answers

### Orbital period required:
$$
\boxed{T = 24\ \text{hours (sidereal: }86164\ \text{s)}}
$$

### Geostationary altitude:
$$
\boxed{h \approx 35,786\ \text{km}}
$$

---

## 7. Key Idea

- The satellite must match Earth’s rotation
- This fixes the orbital radius uniquely
- That’s why all geostationary satellites sit at the same altitude
