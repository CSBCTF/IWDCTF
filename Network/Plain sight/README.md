Message: A person called the incident responder to notify of a hacking incident. The incident responder has acquired the pcap file which is soon to be analyses.  

Can you find out the Victim ip address?

Format flag: IWDCTF{ip address}
Value: 50

In this challenge, a pcap file was provided containing the network traffic. From the Tcp follow stream we can see that this is a Phishing scam. 

<img src="https://github.com/CSBCTF/IWDCTF/blob/8529ff1cb76564421dd187bac095a0b28c5f80a6/Network/Plain%20sight/files/1.png">
 
From the question, we need to find the victim Ip address. At first glance, we can see that ip address 192.168.147.137 is requesting to access a website at 192.168.247.128 via GET request.
By assumption and we can try and submit that ip address in a format flag IWDCTF{192.168.247.137}. It is correct!
