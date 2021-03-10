Rope

Message: Super Advance Vault

Value: 50

We can see that the nature of the file is a Linux executable 64-bit architecture. Which means it’s for Linux OS. 
<img src="https://github.com/CSBCTF/IWDCTF/blob/85aefd446267f124cdbd733f02000a30b550c295/Binary/Rope/files/1%20file.PNG">


Output of the program when ran on Linux OS.
<img src="https://github.com/CSBCTF/IWDCTF/blob/85aefd446267f124cdbd733f02000a30b550c295/Binary/Rope/files/2%20run.PNG">

It seems like it requires a login credentials. When tested with dummy credentials, it output “user doesn’t exist” prompt. Let’s see if we can look what is inside of the file.  

We can use strings command
<img src="https://github.com/CSBCTF/IWDCTF/blob/85aefd446267f124cdbd733f02000a30b550c295/Binary/Rope/files/3%20strings.PNG">
 
Voilà we can see the flag!
Flag: IWDCTF{0bfU51c@+1on_15_1mP0r+@n+}
