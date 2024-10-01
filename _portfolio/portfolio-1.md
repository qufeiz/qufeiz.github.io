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
