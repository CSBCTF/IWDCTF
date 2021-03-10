Message: Time is merely an illusion

Value: 150 

Identifying file type.
<img src="https://github.com/CSBCTF/IWDCTF/blob/d673519da347cfa18b29e2a39b850360b7c5cadc/Binary%20-%20Time%20Travel/0%20file.PNG">
 
 What can we see from above, the file is a Linux executable with 64-bit architecture. The interesting part is at the end. It shows that this file is stripped. Basically, it means the file is obfuscated and a lot harder to debug since the debugging info has been stripped.

Let’s run the file.

<img src="https://github.com/CSBCTF/IWDCTF/blob/d5cffaa49c9042e27c97888ee27e3be6b59c8bae/Binary%20-%20Time%20Travel/1%20run.PNG">
 
The program shows that this executable has expire, and possibly cannot be run anymore. Something like trial program that has expire where none of us wanted to pay for and just create a new account to get free 30-day trial. Although this might just be a little different. 
From what we gather, the file expires on 28/2/2021. Which means we need to run the program before that date… but how!? It almost doesn’t make any sense. But as we know it...time works differently on different space.  Afterall, time is merely an illusion, as famously quoted by Carlo Rovelli, a theoretical physicist. 

Let go back in time! Or so 

<img src="https://github.com/CSBCTF/IWDCTF/blob/d5cffaa49c9042e27c97888ee27e3be6b59c8bae/Binary%20-%20Time%20Travel/2%20run.PNG">
 
This command above changes the date of the OS to the day before the file expire. Let’s run the file again.
<img src="https://github.com/CSBCTF/IWDCTF/blob/d5cffaa49c9042e27c97888ee27e3be6b59c8bae/Binary%20-%20Time%20Travel/3%20run.PNG">

 It works like a charm. The flag is IWDCTF{s3cr3t_s0ci3ty}
