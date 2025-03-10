# Problem 1
# **Projectile Motion: Theoretical Foundation**

## **1. Governing Equations of Motion**

Projectile motion follows Newton's laws of motion and assumes motion under uniform gravitational acceleration with no air resistance. The fundamental equations arise from Newton’s Second Law:

\[ \mathbf{F} = m\mathbf{a} \]

Since the only force acting on the projectile (neglecting air resistance) is gravity, we have:

\[ F_y = -mg, \quad F_x = 0 \]

Thus, the equations of motion can be written as:

\[ m a_x = 0 \quad \Rightarrow \quad a_x = 0 \]
\[ m a_y = -mg \quad \Rightarrow \quad a_y = -g \]

Since acceleration is the second derivative of position, we get:

\[ \frac{d^2x}{dt^2} = 0, \quad \frac{d^2y}{dt^2} = -g \]

## **2. Solving the Differential Equations**

### **Horizontal Motion**

Integrating the horizontal acceleration equation:

\[ \frac{dv_x}{dt} = 0 \]

\[ v_x = v_0 \cos \theta \]

Since velocity is the derivative of position:

\[ \frac{dx}{dt} = v_0 \cos \theta \]

Integrating again:

\[ x(t) = v_0 \cos \theta \cdot t \]

### **Vertical Motion**

Integrating the vertical acceleration equation:

\[ \frac{dv_y}{dt} = -g \]

\[ v_y = v_0 \sin \theta - gt \]

Since velocity is the derivative of position:

\[ \frac{dy}{dt} = v_0 \sin \theta - gt \]

Integrating again:

\[ y(t) = v_0 \sin \theta \cdot t - \frac{1}{2} g t^2 \]

## **3. Range of the Projectile**

The range \( R \) is the horizontal distance the projectile travels before hitting the ground (i.e., when \( y = 0 \)).

Setting \( y(t) = 0 \):

\[ 0 = v_0 \sin \theta \cdot t - \frac{1}{2} g t^2 \]

Solving for \( t \), we get:

\[ t = \frac{2 v_0 \sin \theta}{g} \]

Substituting into the equation for \( x(t) \):

\[ R = v_0 \cos \theta \cdot \frac{2 v_0 \sin \theta}{g} \]

Using the identity \( 2 \sin \theta \cos \theta = \sin 2\theta \), we obtain the range formula:

\[ R = \frac{v_0^2 \sin 2\theta}{g} \]

## **4. Family of Solutions and Dependence on Initial Conditions**

- The range depends on both the initial velocity \( v_0 \) and the launch angle \( \theta \).
- The **maximum range** occurs at \( \theta = 45^\circ \), since \( \sin 2\theta \) is maximized at \( 90^\circ \).
- The **same range** can be achieved with complementary angles \( \theta_1 \) and \( \theta_2 = 90^\circ - \theta_1 \), as \( \sin 2\theta \) is the same for both.

### **Effect of Gravity**

- Increasing gravity \( g \) decreases the range since \( R \propto 1/g \).
- Lower gravity environments (e.g., Moon or Mars) allow longer ranges for the same launch velocity.

### **Effect of Initial Velocity**

- The range is **quadratic** in \( v_0 \), meaning a slight increase in velocity results in a significantly larger range.

## **Conclusion**

The projectile motion equations provide deep insight into real-world applications, from sports physics to space exploration. The range formula highlights the key dependencies on angle, velocity, and gravity, illustrating the elegance of motion under constant acceleration.


