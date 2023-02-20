---
layout: page
title: Multicore Processor on FPGA
nav-menu: false
show_tile: false
---

<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Multicore Processor on FPGA</h1>
		</header>

<!-- Content -->
Designing and implmenting a pipelined, multicore processor with cache coherency remains one of the most difficult yet rewarding projects of my life. Purdue is the only university in the country that offers a course dedicated to such an extensive FPGA project. Prior to this class, I studied digital design on FPGA boards in two semesters of undergraduate ASIC design courses. I also wrote dual thread programs in the assembly language MIPS to test my designs.<br><br>
My teammate and I recorded the maximum clock frequency and clock cycle used in gate level simulations and computed both the Instruction Latency (IL) and the number of Millions Instructions Per Second (MIPS) to compare our designs with and without caches. The benchmark program we used throughout testing was merge sort. This program's instruction count is 5404 in the single thread version and 5421 in the dual thread version.<br><br>
		
<center><img src="assets/images/multicore_FBD.jpg" alt="Multicore FBD" width="800"></center>
<center><b>Figure 1.</b> Functional block diagram of the pipelined multicore processor with caches.</center>
		<br>
<center><img src="assets/images/multicore_perf.png" alt="Multicore Performance Results" width="500"></center>
<center><b>Figure 2.</b> Results from quantitatively comparing our designs with and without caches.</center>
		
