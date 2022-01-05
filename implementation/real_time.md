# Real-Time Systems

Most embedded computing tasks have a [deadline][1], but the consequences of missing this deadline vary depending on the application. This leads to a natural classification of systems based on the severity consequence for missing the deadline.

**Hard** – Missing the deadline is a total system failure. Example: deployment of a car airbag.

**Firm** – Missing the deadline makes the system useless, but there is an opportunity to retry or correct the result. Example: on a printer, missing a deadline of depositing ink may completely ruin the result, but the print can be restarted or corrected by hand.

**Soft** – Missing the deadline makes the system less useful, but it is still better than having no result at all. Example: frame update in a video game.

Systems with a deadline are said to be [real-time][2]. Systems with a soft deadline can be run on a smartphone, PC, or single-board computer running a general purpose operating system. Systems with hard or firm deadlines are typically executed on [bare metal][3]. The presence of an operating system influences the type of processor that can be used, since most operating systems require a [memory management unit][4].

[1]:https://en.wikipedia.org/wiki/Time_limit
[2]:https://en.wikipedia.org/wiki/Real-time_computing
[3]:https://en.wikipedia.org/wiki/Bare_machine
[4]:https://en.wikipedia.org/wiki/Memory_management_unit

| Processor Type	| Example application	| Memory Management Unit	| Approximate Power (Watts) | Approximate performance (MIPS)|
| :---        		| :----:   				| :----:   					| :----:   					| :----:						|
| ARM Cortex-M   	| Automotive			| No						| 0.1	  					| 100							|
| ARM Cortex-A   	| Smartphone			| Yes   					| 1							| 1000							|
| TI C6000     		| Medical Imaging		| No	  					| 3		   					| 5000							|
| Intel Core i5		| Desktop PC			| Yes	 					| 50	   					| 100000						|


