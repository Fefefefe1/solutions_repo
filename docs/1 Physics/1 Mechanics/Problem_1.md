# Problem 1
Problem 1¶

Investigating the Range as a Function of the Angle of Projection

Motivation:¶

Projectile motion, while seemingly simple, offers a rich playground for exploring fundamental principles of physics. The problem is straightforward: analyze how the range of a projectile depends on its angle of projection. Yet, beneath this simplicity lies a complex and versatile framework. The equations governing projectile motion involve both linear and quadratic relationships, making them accessible yet deeply insightful.

What makes this topic particularly compelling is the number of free parameters involved in these equations, such as initial velocity, gravitational acceleration, and launch height. These parameters give rise to a diverse set of solutions that can describe a wide array of real-world phenomena, from the arc of a soccer ball to the trajectory of a rocket.

Task:¶

1 Theoretical Foundation:

Begin by deriving the governing equations of motion from fundamental principles. This involves solving a basic differential equation to establish the general form of the motion.
Highlight how variations in initial conditions lead to a family of solutions.
2 Analysis of the Range:

Investigate how the horizontal range depends on the angle of projection.
Discuss how changes in other parameters, such as initial velocity and gravitational acceleration, influence the relationship.
3 Practical Applications:

Reflect on how this model can be adapted to describe various real-world situations, such as projectiles launched on uneven terrain or in the presence of air resistance.
4 Implementation:

Develop a computational tool or algorithm to simulate projectile motion.
Visualize the range as a function of the angle of projection for different sets of initial conditions.
Deliverables:¶
A Markdown document with Python script or notebook implementing the simulations.
A detailed description of the family of solutions derived from the governing equations.
Graphical representations of the range versus angle of projection, highlighting how different parameters influence the curve.
A discussion on the limitations of the idealized model and suggestions for incorporating more realistic factors, such as drag or wind.
Hints and Resources:¶
Start from the fundamental laws of motion and gradually build the general solution.
Use numerical methods or simulation tools to explore scenarios that go beyond simple analytical solutions.
Consider how this model connects to real-world systems, such as sports, engineering, and astrophysics.
This task encourages a deep understanding of projectile motion while showcasing its versatility and applicability across various domains.^^^^
### There Is The Answer And The Calculation Codes For The Questions
import numpy as np
import matplotlib.pyplot as plt

def projectile_motion(v0, theta, g=9.81):
    """
    Computes the range, maximum height, and flight time of a projectile.
    :param v0: Initial velocity (m/s)
    :param theta: Launch angle (degrees)
    :param g: Acceleration due to gravity (m/s^2), default is 9.81 m/s^2
    :return: (range, max_height, flight_time)
    """
    theta_rad = np.radians(theta)
    range_ = (v0**2 * np.sin(2 * theta_rad)) / g
    max_height = (v0**2 * (np.sin(theta_rad))**2) / (2 * g)
    flight_time = (2 * v0 * np.sin(theta_rad)) / g
    return range_, max_height, flight_time

# Define parameters
v0 = 20  # Initial velocity in m/s
angles = np.linspace(0, 90, num=100)  # Angle range from 0 to 90 degrees
ranges = []
max_heights = []
flight_times = []

for theta in angles:
    r, h, t = projectile_motion(v0, theta)
    ranges.append(r)
    max_heights.append(h)
    flight_times.append(t)

# Plot results
plt.figure(figsize=(8, 5))
plt.plot(angles, ranges, label='Range (m)')
plt.plot(angles, max_heights, label='Max Height (m)')
plt.plot(angles, flight_times, label='Flight Time (s)')
plt.xlabel('Launch Angle (degrees)')
plt.ylabel('Value')
plt.title('Projectile Motion Analysis')
plt.legend()
plt.grid()
plt.show()

