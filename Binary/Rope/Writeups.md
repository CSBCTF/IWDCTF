Rope

Message: Super Advance Vault

Value: 50

We can see that the nature of the file is a Linux executable 64-bit architecture. Which means it’s for Linux OS. 
<img src="https://github.com/CSBCTF/IWDCTF/blob/790152cb1ebc6394ca7836725e586678d9ac64fe/Binary%20-%20Rope/1%20file.PNG">


Output of the program when ran on Linux OS.
<img src="https://github.com/CSBCTF/IWDCTF/blob/f11a4497d8881f703a840036d9dcd5ad12f65e0c/Binary%20-%20Rope/2%20run.PNG">

It seems like it requires a login credentials. When tested with dummy credentials, it output “user doesn’t exist” prompt. Let’s see if we can look what is inside of the file.  

We can use strings command
<img src="https://github.com/CSBCTF/IWDCTF/blob/fecf28220c0613d17f60789affc229c88e391eb4/Binary%20-%20Rope/3%20strings.PNG">
 
Voilà we can see the flag!
Flag: IWDCTF{0bfU51c@+1on_15_1mP0r+@n+}
