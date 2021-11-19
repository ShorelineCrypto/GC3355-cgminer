# GC3355-cgminer
cgminer for Gridseed devices

Usage:

First run the AutoInstaller to compile and install cgminer.

	$ ./RPi-AutoInstaller

Wait for the AutoInstaller to finish and then use the Worker Generator to make executable bash file for running miner.

	$ ./Worker-Generator

First, choose a name for the bash script to be saved as, no spaces allowed.

	  Save As:
	  Exampe
Second, select algo

	  Pool Algo:
	  sha256
	  or
	  scrypt
	  scrypt

Third, Insert chosen scrypt pool url.

	  Pool URL:
	  stratum+tcp://us2.litecoinpool.org:3333

Fourth, Insert worker name for selected pool.

	  Pool Worker:
	  Meap10.Test

Fifth, Insert worker password.

	  Worker Password:
	  x

Fifth, Select the Frequency. 850 is recommended for a hashrate of 350 khs

	  Orb Frequency:
	  Can be 600, 625, 650, 675, 700, 725, 750, 775, 800, 825, 850, 875, 900
	  **Recommended Frequency is 850**
	  850

Once that's done, run the script just made with a ./ infront of the name.

	$ ./Example

If all is done well, you should see something like this.


	   cgminer version 4.3.5 - Started: [2021-11-19 11:53:54]
	  --------------------------------------------------------------------------------
	   (5s):360.1K (avg):360.0Kh/s | A:768  R:0  HW:0  WU:1.1/m
	   ST: 2  SS: 0  NB: 2  LW: 31  GF: 0  RF: 0
	   Connected to us2.litecoinpool.org diff 256 with stratum as user Meap10.Test
	   Block: a552a120...  Diff:11.7M  Started: [22:18:51]  Best share: 351
	  --------------------------------------------------------------------------------
	   [P]ool management [S]ettings [D]isplay options [Q]uit
	   GSD 0: 6D9214984857  850 MHz | 360.0K/366.5Kh/s | A:768 R:0 HW:0 WU:1.1/m
	  --------------------------------------------------------------------------------

	   [2021-11-16 22:18:35] Started cgminer 4.3.5
	   [2021-11-16 22:18:36] GridSeed options: 'baud=115200,freq=850,chips=5,usefifo=0,btc=16'
	   [2021-11-16 22:18:36] Device found, firmware version 01140113, driver version v3.8.5.20140210.02
	   [2021-11-16 22:18:36] System reseting
	   [2021-11-16 22:18:36] Set GC3355 core frequency to 850 MHz
	   [2021-11-16 22:18:36] Probing for an alive pool
	   [2021-11-16 22:18:37] Pool 0 difficulty changed to 65536
	   [2021-11-16 22:18:40] Network diff set to 11.7M
	   [2021-11-16 22:18:44] Pool 0 difficulty changed to 256
	   [2021-11-16 22:18:51] Stratum from pool 0 detected new block
	   [2021-11-16 22:18:51] Stratum from pool 0 requested work restart
	   [2021-11-16 22:18:53] Accepted baf11c43 Diff 351/256 GSD 0
	   [2021-11-16 22:19:01] Accepted e22c607d Diff 290/256 GSD 0
	   [2021-11-16 22:20:30] Stratum from pool 0 requested work restart
	   [2021-11-16 22:20:54] Accepted f93be071 Diff 263/256 GSD 0
