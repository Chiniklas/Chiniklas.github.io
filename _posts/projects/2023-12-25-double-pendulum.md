---
layout: default
title: "Reinforcement learning based control of an underactuated double pendulum system"
date: 2023-12-25
category: projects
image: /images/display_images/double-pendulum.gif
authors: "<strong>Chi Zhang</strong>"
advisor: "Felix Wiebe, Akhil Sathuluri, Prof. Dr. Shivesh Kumar, Prof. Dr. Frank Kirchner, Prof. Dr. Markus Zimmermann"
venue: "Master Thesis, Robotics Innovation Center, DFKI GmbH"
preprint: pre_print/solving_the_swing-up_and_balance_task_for_the_acrobot_and_pendubot_with_SAC.pdf
code: https://github.com/Chiniklas/double_pendulum
---
In this project, reinforcement learning-based control was attempted on an underactuated double pendulum system to perform the tasks of swinging up and stabilization. Depending on the joint being controlled, the systems are referred to as the 'pendubot' and the 'acrobot.' A combined controller consisting of an RL agent trained with the Soft Actor-Critic (SAC) algorithm for the swing-up task and a Linear Quadratic Regulator (LQR) for stabilization is employed. A 3-stage reward function was designed to guide the agent into the Region of Attraction (RoA) of the LQR controller, where the system achieves asymptotic stability toward the goal state and maintains stability over an extended duration.<br><br>
Validation in an ideal environment, without real-world features such as friction, torque responsiveness, measurement noise, and signal delay, was successful. During the real hardware phase, a noisy simulation was established to mimic these real-world conditions before transferring the controller to real hardware. To address the sim-to-real gap, a noisy training process based on domain randomization was implemented to enhance robustness. The SAC+LQR controller, which demonstrated a 40% success rate on a real pendubot setup, was evaluated in terms of performance and robustness based on results from both simulations and real-world tests, with quantitative metrics reflected on the respective leaderboards.<br><br>
The results were presented at IJCAI 2023 to participate in the RealAIGym competition. Details can be found in the pre-print.