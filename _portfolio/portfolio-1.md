---
title: "Portfolio item number 1"
excerpt: "Short description of portfolio item number 1<br/><img src='/images/500x300.png'>"
collection: portfolio
---

This is an item in your portfolio. It can be have images or nice text. If you name the file .md, it will be parsed as markdown. If you name the file .html, it will be parsed as HTML. 

Wheeled Inverted Pendulum Control and Dynamics Simulation (MATLAB/Simulink)

Developed a dynamic model of a wheeled inverted pendulum using Lagrangian mechanics.
Derived and implemented non-linear equations of motion for a complex coupled system.
Simulated and solved the system's dynamics using MATLAB, including mass matrices and external force vectors.
Extended the model to design feedback control for stability using PID/LQR (optional).

Wheeled Inverted Pendulum Dynamics and Control Simulation
Project Overview: In this project, I modeled and simulated the dynamics of a wheeled inverted pendulum, a classic problem in control theory and robotics. This system, often used to model self-balancing robots (such as Segways), presents a significant challenge due to its inherent instability and non-linear dynamics. The project involved deriving the equations of motion using Lagrangian mechanics, developing a mathematical model of the system, and implementing this model in MATLAB/Simulink to analyze its behavior.

Key Components:

Lagrangian Dynamics: The dynamics of the wheeled inverted pendulum were derived using the Lagrangian formulation, which is based on the system's kinetic and potential energy. This allowed me to describe the coupled relationship between the wheel's rotation and the pendulum's pitch angle using differential equations. The complexity arises from the interaction between the rotational motion of the wheel and the pendulum's pivot point, making this a classic example of a multi-degree-of-freedom system.

Equations of Motion: I derived the non-linear Euler-Lagrange equations that govern the motion of the system. These equations describe how the angular accelerations of the wheel and the pendulum respond to applied torques, gravitational forces, and inertial forces. The result was a set of coupled second-order differential equations that were solved using MATLAB's symbolic toolbox.

Mass Matrix and Forcing Vector: From the equations of motion, I identified the mass matrix (A) and the forcing vector (B), representing the system's inertia and external forces, respectively. These matrices were then used to solve for the angular accelerations of the system. By structuring the equations in matrix form, I could implement them efficiently in MATLAB, enabling dynamic simulation of the system under various input conditions.

Numerical Simulation: Using MATLAB/Simulink, I implemented the derived equations to simulate the dynamic behavior of the pendulum. This simulation accounted for:

The non-linear coupling between the wheel's angular motion and the pendulum's pitch.
The influence of external forces, such as gravity and applied torque.
Real-world factors like the Coriolis effect and gravitational forces acting on the pendulum.
Control System Design (Optional Extension): As an extension, I implemented a feedback control system to stabilize the pendulum. This involved designing a PID controller to ensure the pendulum remains upright while the system is subjected to various disturbances. The controller was tuned to provide stable responses and smooth control of the system.

Challenges and Solutions:

Non-Linear Dynamics: One of the primary challenges was dealing with the non-linear nature of the system. The pendulum's behavior is highly sensitive to initial conditions, and without proper control, the system becomes unstable. I tackled this by linearizing the equations around the upright equilibrium point for control purposes and using numerical methods to handle the full non-linear model.

Energy Conservation and Stability: During simulation, it was critical to ensure that the energy dynamics of the system were properly captured. I carefully derived the kinetic and potential energy expressions, ensuring that the energy flows in the system were consistent with physical principles. This was particularly important when analyzing the stability and control aspects of the pendulum.

Simulation Efficiency: The model was optimized for simulation efficiency by organizing the equations into matrix form. This allowed for more rapid numerical integration of the equations, which was crucial for real-time simulation and control testing.

Project Outcomes:

Developed a complete mathematical model of the wheeled inverted pendulum using Lagrangian mechanics.
Implemented the system’s equations of motion in MATLAB, solving for the angular accelerations and simulating the system's behavior.
(Optional) Designed and tuned a feedback control system to stabilize the pendulum, ensuring it remained upright under varying conditions.
Demonstrated the use of advanced mathematical techniques to model and control a real-world dynamic system, showing proficiency in both physics-based modeling and control theory.
Applications: The wheeled inverted pendulum model has numerous real-world applications, including:

Robotics: It forms the basis of self-balancing robots like Segways or robotic unicycles.
Control System Design: The control challenges presented by this system are typical of many unstable systems, making it an excellent testbed for developing robust controllers.
Dynamic System Simulation: Understanding the behavior of coupled dynamic systems is essential for many engineering fields, including automotive, aerospace, and mechanical engineering.
Technologies Used:

MATLAB: For symbolic derivation of the equations of motion and numerical simulations.
Simulink: For implementing the dynamic simulation and designing the control system.
Control Theory: To design a feedback system that stabilizes the pendulum in real time.

Self-Balancing Robot with Extended Kalman Filter and Trajectory Control
Project Overview:
In this project, I developed a self-balancing two-wheeled robot utilizing an Extended Kalman Filter (EKF) to estimate the system states from noisy sensor data, and implemented a Proportional-Derivative (PD) controller to maintain balance and follow a desired trajectory. The system was modeled and simulated using MATLAB/Simulink, and the control algorithm was designed to ensure smooth and accurate tracking of predefined paths.

Key Objectives:
Design a state estimation algorithm using an Extended Kalman Filter (EKF) to handle noisy sensor inputs from accelerometers and gyroscopes.
Implement a PD controller for balance control and trajectory tracking based on sensor feedback.
Simulate and test the system in MATLAB to ensure robust performance under varying conditions, including noisy environments and real-world uncertainties.
My Role:
As the lead developer of this project, I was responsible for the entire workflow—from system modeling to implementation, testing, and performance tuning. I leveraged the following skills to achieve the project goals:

Control System Design: Implemented a cascade control architecture with inner-loop balancing and outer-loop trajectory tracking.
State Estimation: Developed the EKF to filter out noise from sensors and accurately estimate the robot's roll angle (
𝜙
ϕ) and angular velocity (
𝜙
˙
ϕ
˙
​
 ).
Trajectory Tracking: Integrated trajectory control using wheel encoders and calculated desired body angles (
𝜙
des
ϕ 
des
​
 ) to ensure smooth movement along a predefined path.
Noise Handling: Tuned the EKF's process and measurement noise covariances to improve stability and noise robustness in real-time scenarios.
Technical Challenges:
Noisy Sensor Data:

The robot’s accelerometer and gyroscope readings were subject to noise, making direct control challenging. I addressed this by designing and fine-tuning the EKF to estimate the roll angle and angular velocity from the noisy measurements.
Non-linear Dynamics:

Balancing a two-wheeled robot involves non-linear dynamics, especially when the system deviates significantly from the upright position. By incorporating a non-linear control law using the sine function, I ensured that the system could handle larger angle deviations smoothly.
Trajectory Control:

The robot needed to follow a predefined path while maintaining balance. This required designing an outer-loop PD controller that calculated the desired body angle 
𝜙
des
ϕ 
des
​
  based on the robot's position 
𝑥
x and velocity 
𝑥
˙
x
˙
 , and an inner-loop PD controller to balance the robot using real-time feedback.
Tools & Technologies:
MATLAB/Simulink for system modeling, simulation, and control design.
State Estimation using Extended Kalman Filters (EKF) to estimate the roll angle and angular velocity from accelerometer and gyroscope data.
Control Theory: Cascade PD control structure for balancing and trajectory tracking.
Signal Processing: Filter design and noise rejection techniques for sensor data.

Outcomes:
Stable Balance Control:

Successfully implemented a robust balance control system that maintained the robot in an upright position even under significant disturbances and noisy sensor readings. The EKF effectively filtered out the noise, enabling accurate state estimation for the controller.
Accurate Trajectory Tracking:

The robot was able to follow a desired trajectory (such as a sinusoidal or step response) while maintaining balance. The PD controller, combined with the wheel encoder readings, ensured precise movement along the trajectory, with minimal deviation from the target.
Noise Robustness:

The EKF significantly improved the system's ability to operate in noisy environments, filtering out sensor noise and enabling the robot to make smooth and reliable control decisions. This made the system more practical for real-world deployment where sensor noise is inevitable.
Refined Control Gains:

Through extensive testing and simulation, I was able to fine-tune the proportional and derivative control gains for both the balancing and trajectory control loops, optimizing the robot's responsiveness and stability.
What I Learned:
Advanced Control Theory: This project deepened my understanding of control system design, particularly how to handle non-linear dynamics and combine state estimation with real-time control for complex systems.
State Estimation Techniques: Working with the Extended Kalman Filter taught me how to estimate system states accurately in the presence of noise, a key skill in robotics and autonomous systems.
Iterative Tuning: I gained hands-on experience in tuning control parameters and noise covariances to achieve the desired system performance, balancing responsiveness with stability.
MATLAB/Simulink Proficiency: I developed a strong command over MATLAB/Simulink for simulation and testing, learning how to effectively model dynamic systems, simulate sensor inputs, and visualize system performance.
Potential Applications:
Autonomous Robots: The techniques developed in this project can be applied to balance control in two-wheeled robots or other dynamically unstable platforms such as hoverboards, self-balancing scooters, or robotic manipulators.
Self-Driving Vehicles: The state estimation and control strategies are highly transferable to autonomous systems, such as drones, self-driving cars, and other vehicles that require precise control under noisy conditions.
Key Skills Developed:
State Estimation: Expertise in implementing Extended Kalman Filters (EKF) for filtering noisy sensor data and accurately estimating system states.
Control Systems: Advanced understanding of PID and PD controllers, including non-linear control techniques for dynamically unstable systems.
Simulation and Modeling: Proficient in using MATLAB/Simulink for dynamic system simulation, modeling, and control validation.
Signal Processing: Experience in handling noisy sensor data and implementing filtering techniques to improve system robustness.
Visuals (Optional for Portfolio Website):
Simulation Results: Include graphs showing the robot's roll angle, angular velocity, and trajectory tracking performance over time.
System Diagram: A block diagram showing the flow of sensor data through the EKF, and how the controller computes the control inputs based on the estimated states and desired trajectory.
