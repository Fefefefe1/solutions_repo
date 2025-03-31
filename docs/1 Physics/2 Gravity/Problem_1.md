# Problem 1
# Derivation of Kepler's Third Law

## Horizontal Motion

Since velocity is the derivative of position:

$$
\frac{dx}{dt} = v_0 \cos\theta
$$

Integrating again:

$$x(t) = v_0 \cos\theta \cdot t
$$

### **Vertical Motion**

Integrating the vertical acceleration equation:

$$
\frac{dv_y}{dt} = -g
$$

The velocity in the vertical direction is:

$$
v_y = v_0 \sin\theta - gt
$$

Since velocity is the derivative of position:

$$
\frac{dy}{dt} = v_0 \sin\theta - gt
$$
# Astronomical Implications

## Planetary Masses

Kepler's Third Law can be used to calculate the mass of a planet or a star if we know the orbital period and the orbital radius of a satellite or planet in orbit. Rearranging the derived equation:

$$
T^2 = \frac{4\pi^2 r^3}{GM}
$$

We can solve for the mass \( M \):

$$
M = \frac{4\pi^2 r^3}{GT^2}
$$

This formula allows us to calculate the mass of the central object (like a planet or a star) using the orbital period \( T \) and the orbital radius \( r \) of an orbiting body. For example, if we know the orbital characteristics of a satellite or moon, we can determine the mass of the planet or star it orbits.

## Orbital Distances

Kepler's Third Law also helps us calculate the orbital distance (semi
# Real-World Analysis

## Moon's Orbit Around Earth

Kepler's Third Law allows us to analyze the Moon's orbit around Earth by using the known orbital period and orbital radius. The Moon’s orbital period is approximately 27.32 days, and the average distance from Earth is about 384,400 km.

To calculate the mass of Earth using Kepler's Third Law, we can rearrange the formula:

$$
M = \frac{4\pi^2 r^3}{GT^2}
$$

Where:
- \( r = 384,400 \, \text{km} \) (orbital radius),
- \( T = 27.32 \, \text{days} \) (orbital period, which we convert to seconds for consistency).

Using the known gravitational constant \( G \), we can solve for the mass of Earth. This illustrates how Kepler's Third Law can be used to determine the mass of a planet or moon based on orbital parameters.

## Orbits of Planets in the Solar System

Kepler’s Third Law is crucial in understanding the motion of planets in the Solar System. By analyzing the orbital periods and radii of planets, we can infer various important properties.

For example, the orbital period of Earth is 1 year, and its average orbital radius (semi-major axis) is 1 Astronomical Unit (AU) or 149.6 million km. If we apply Kepler's Third Law, we can calculate the mass of the Sun.

For a planet like Jupiter, which has an orbital period of about 11.86 years and an average orbital radius of 5.2 AU, we can use Kepler's Third Law to verify its motion relative to the Sun. By comparing the orbital parameters of all planets, we see that the farther a planet is from the Sun, the longer its orbital period, which is consistent with the relationship \( T^2 \propto r^3 \).


### Codes Of Tables
import pandas as pd


### Tables

#### Table 1: Orbital Period and Radius

| Planet  | Orbital Period (years) | Orbital Radius (AU) |
|---------|------------------------|---------------------|
| Earth   | 1.00                   | 1.000               |
| Mars    | 1.88                   | 1.524               |
| Jupiter | 11.86                  | 5.203               |
| Saturn  | 29.46                  | 9.537               |

#### Table 2: Orbital Characteristics of Moons

| Moon   | Orbital Period (days) | Orbital Radius (km) |
|--------|-----------------------|---------------------|
| Moon   | 27.32                 | 384400              |
| Phobos | 0.32                  | 9377                |
| Europa | 3.55                  | 671100              |
| Titan  | 15.95                 | 1221870             |

![alt text](image-1.png) 

