Packet Analysis
Question:
“Women in leadership: Achieving an equal future in a COVID-19 world”

Value: 100
Solution:
1.	Filter PCAP = Frame contains Women
 <img src="https://github.com/CSBCTF/IWDCTF/blob/8e969abf9ac4fcafee3b061741b178cde082371b/Network/Women/files/1.png">
We get 3 IPs involved 
	192.168.57.3 (Host)
	192.168.57.4 (Web Server)
	192.168.57.5 (Actual Web Server)
2.	Follow TCP Stream for each server and each packet that connect with host until reach IWD/IWD/Index.html 
 <img src="https://github.com/CSBCTF/IWDCTF/blob/8e969abf9ac4fcafee3b061741b178cde082371b/Network/Women/files/2.png">
3.	Open TCP Stream for the packet 
4.	Get the code from TCP Stream
 <img src="https://github.com/CSBCTF/IWDCTF/blob/8e969abf9ac4fcafee3b061741b178cde082371b/Network/Women/files/3.png">
 
5.	Convert Code with Base 64 using base64decode.org
 <img src="https://github.com/CSBCTF/IWDCTF/blob/8e969abf9ac4fcafee3b061741b178cde082371b/Network/Women/files/4.png">
 
6.	Get the Flag

The Flag is IWDCTF{w0m3n_1n_L34D3r5h1p}
