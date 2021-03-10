Message: Due to the pandemic, Joker has changed his career path to cybercrime.  He finally got something after few months of trying to get into Justice League system. Now, he is stuck and did not know what to do next.

Value: 75

LLMNR is a protocol that is use in Active directory. 

<img src="https://github.com/CSBCTF/IWDCTF/blob/9bd743a1388502c9a19864eef7de6a8844a517f4/Crypto/LLMNR/files/1.PNG">

Above is the attached file. 
 It looks like a hash. 

Since this challenge is named LLMNR, we can safely assume it is a hash captured from Active directory. This hash needed to be cracked. One of the tools used for hash cracking is hashcat. The hash looks similar to NTLMv2 hash. We can know by googling type of hashes from LLMNR and Active Directory and NTLMV2 hash looks the closes to this hash.

Hashcat command to crack NTLMV2 hash
<img src="https://github.com/CSBCTF/IWDCTF/blob/9bd743a1388502c9a19864eef7de6a8844a517f4/Crypto/LLMNR/files/2.PNG">
 
Command:
 Hashcat – cracking tools
-m 5600 – referring to NTLMV2 hash
home/kali/Desktop/JusticeLeaguePC.txt – the file containing hash
home/kali/Desktop/rockyou.txt – wordlist required to compare the hash to.

Results of hashcat

<img src="https://github.com/CSBCTF/IWDCTF/blob/9bd743a1388502c9a19864eef7de6a8844a517f4/Crypto/LLMNR/files/1.PNG">
The hash has been cracked! 
Its 12#$qwER.

Flag: IWDCTF{12#$qwER}
