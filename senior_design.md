---
layout: page
title: Robotic Arm with Inverse Kinematics
description: Senior Design Project
nav-menu: false
show_tile: false
---

<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Advanced Robotic Arm</h1>
		</header>

<!-- Content -->

The robotic arm takes a coordinate provided by the user and determines the optimal combination of angles to move its end-effector as desired. It can also trace and reproduce movements by recording the angles of the revolute joints over time. The mechanical structure boasts augmented stability and force multiplication due to the cabling linkages located at each joint. This design incorporates biomimicry by imitating the flexion-extension system of ligaments through pulleys and tensioned cables. Additionally, a Raspberry Pi is used to display a user interface, stream sensor data in real time, locate and identify objects through a camera, and even simulate how the arm is expected to move in 3-dimensional space. We were able to scale the raw gyroscope and acceleration data from the IMU and plot the data points live through the Raspberry Pi. The IMU also has EMI protection, and most of the traces on the PCB have ESD protection to ensure the safety and reliability of the components. Finally, we simulated all mechanical movements in Python before construction by modeling the inverse kinematics algorithm.

This robotic limb is meant to function as a building block for constructing walking robots. It is specially designed as a hexapod leg for traversing non-planar environments, but its possible applications in industry are endless.

<img src="arm_render.jpg" alt="Robotic Arm Render">
