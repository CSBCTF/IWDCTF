
Challenge: Up 
<br>
Message: http://csb.iwdctf.xyz:8082
<br>
Value: 100

<img src= "https://github.com/CSBCTF/IWDCTF/blob/e605738d6379d5543af5770eb95a0fcdaf416caa/web/up/files/Capture.PNG">

Let's navigate to the page

<img src="https://github.com/CSBCTF/IWDCTF/blob/e605738d6379d5543af5770eb95a0fcdaf416caa/web/up/files/Capture1.PNG">

This is a classic reverse shell upload attack. 
You can find any other script which works in similar way to this one.
<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/CapturePOC.PNG">

Let's upload this shell script that we get from internet.
<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture2.PNG">
<br>
The upload is succesful.
<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture3.PNG">

It shows us where is script is stored.
Let's navigate to the url.

<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture4.PNG">

We can see the script is working. It gaves us terminal.
Executing **ls** command shows all the files in the directory. 

<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture5.PNG">

Let's try directory traversal. 

<img src ="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture6.PNG">

It seems like the command can only be run on a time. Let's try again with multiple command.

This time we include multiple command **cd and ls**

<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture7.PNG">


It takes trial and error to find the flag. This flag.txt seems promising.

<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture9.PNG">

Run **cat /etc/flag.txt**

<img src="https://github.com/CSBCTF/IWDCTF/blob/e7d0af80a54571c6f3f4ba85182f3debf680ea94/web/up/files/Capture10.PNG">

We got the flag: IWDCTF{@lways_S@n!tizE_upl0@ds}



