Message: Waiting game is strong

Value: 250 

File info of waiting.x
<img src="https://github.com/CSBCTF/IWDCTF/blob/79aebcfe90704f4bc23ec4ae7744fd6187d069a4/Binary/Waiting/files/1.PNG">
 

Since the value of this challenge is quite high. It’s surely is tougher. From the info above, the file debug info has been stripped.  

Upon running the program. 

<img src="https://github.com/CSBCTF/IWDCTF/blob/79aebcfe90704f4bc23ec4ae7744fd6187d069a4/Binary/Waiting/files/2.PNG">
 

There program seems to be running on some sort of countdown timer. 25200 seconds until we get the flag (?)
25200 seconds = 7 hours. 
We can just wait it out until it gives us the flag….or maybe we can get to work. 

Let’s open a debugger to debug the program. 
<img src="https://github.com/CSBCTF/IWDCTF/blob/79aebcfe90704f4bc23ec4ae7744fd6187d069a4/Binary/Waiting/files/3.PNG">
 
 From the first look, gdb did not found debugging symbols. Let’s just run the program. 

 <img src="https://github.com/CSBCTF/IWDCTF/blob/79aebcfe90704f4bc23ec4ae7744fd6187d069a4/Binary/Waiting/files/5.PNG">

Seems like the program is still running in the background as the countdown timer is waiting to finish. 
Let’s stop/cancel the program by pressing ctrl+C (kali linux vm on Windows).  After that using the command continue  to resume the program.  
 
<img src="https://github.com/CSBCTF/IWDCTF/blob/79aebcfe90704f4bc23ec4ae7744fd6187d069a4/Binary/Waiting/files/6.png">

As shown above, we just skip the sleep program use for countdown timer and retrieved the flag.
Flag: IWDCTF{t1m3_15_n0t_r3@l}
