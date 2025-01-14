---
layout: page
title: Smart Robotic Arm with Advanced Cabling Linkages
nav-menu: false
show_tile: false
---

<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Smart Robotic Arm with Advanced Cabling Linkages</h1>
		</header>

<!-- Content -->
As project leader, I worked closely with my teammates to design and build the mechanical and electrical components for one of the most ambitious senior design projects at Purdue University. This robotic limb finds the optimal path to any given coordinate and moves its end effector with the help of a revolutionary new elbow joint design. All the motors are centered at the base of the robot and force multiplication in each joint is achieved through pulleys and cabling linkages.<br><br>
	
The robot takes a coordinate provided by the user and determines the optimal combination of angles to move its end effector. It can also trace and reproduce movements by recording the angles of the joints over time. The mechanical structure boasts augmented stability and force multiplication due to the pulley-cabling linkages located at each joint. This design incorporates biomimicry by imitating the flexion-extension system of ligaments through pulleys and tensioned cables.<br><br>
		
Additionally, a Raspberry Pi is used to display a user interface, stream sensor data in real time, locate and identify objects through a camera, and even simulate how the arm is expected to move in 3-dimensional space. We scale the raw gyroscope and acceleration data from the inertial measurement unit (IMU) and plot the data points in real-time through the Raspberry Pi. The IMU has EMI protection and most of the traces on the PCB have ESD protection to ensure the safety and reliability of each component. Finally, we simulated all mechanical movements in Python before construction by modeling the inverse kinematics algorithm.<br><br>
		
This robotic limb is meant to function as a building block for constructing walking robots. It is specially designed as a hexapod leg for traversing non-planar environments, but its possible applications in industry are endless. The cable driven revolute joint was directly inspired by the LIMS2-AMBIDEX arm which was developed by researchers in South Korea. It contains two counteracting pulley sets which use the same cable reel to achieve bending. In this design, augmenting the mechanical advantage is proportional to the number of pulleys and rollers.<br><br>

<center><img src="assets/images/arm_render.png" alt="Robotic Arm Render" width="600"></center>
		<center><b>Figure 1.</b> Rendering of the robotic arm with pulley-cable linkages.</center>

<br>The primary computational engine is a 32-bit, 144-pin microcontroller (STM32F412 MCU) that coordinates and manages data acquisition, digital signal processing, communication, and motor control. Absolute optical encoders mounted on each mechanical joint assembly report the robotic arm position over SPI at any point in time. IMUs, communicating over I2C, allow for the measurement of vibration and mechanical deviation from position determined via optical encoders. Due to drift, IMUs must be re-zeroed when the system is stationary between movement sets.<br><br>

<center><img src="assets/images/arm_fbd.png" alt="Functional Block Diagram" width="600"></center>
		<center><b>Figure 2.</b> Functional block diagram of system components.</center>
		
<br>The pulley-cable system offers a 3:1 mechanical advantage and consequently mitigates the robot's expected power demand. Two 450W parallelized power supplies (SE-450-36) provide sufficient power, while a single 36V, 9.7A supply (LRS-350-36) powers all the electrical systems. A 36V to 5V buck converter supplies the primary rail on the PCB, with additional buck and LDO converters supplying a logic voltage of 3.3V to peripheral systems. The STM32F412 microcontroller consumes about 125 mW of power.
