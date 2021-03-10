Message: Can you find out the attackers ip address?

Value: 50
 
<img src="https://github.com/CSBCTF/IWDCTF/blob/fa9238280767eaec3a87c257fd3c8fbc62f3841e/Network/Plain%20Sight%202/files/2.png">
 
The victim with ip 192.168.247.137 is requesting a HTTP Get request to 192.168.247.128 and the received replied with status 200. Which concludes that ip 192.168.247.128 is the phishing website server. Let’s try submitting the flag IWDCTF{192.168.247.128}. It is correct
