Message: What is the domain name the attacker logged into?
                    Format flag: IWDCTF{subdomain.domain.tld}
Value: 50


Now we need to find the domain name with the format of “subdomain.domain.tld”
 <img src="https://github.com/CSBCTF/IWDCTF/blob/a1af7520b6351d0c60d4149982ab76a74b47943c/Network/Plain%20Sight%203/files/3.png">

Above shows a post request of the phishing website send to the attacker server. Let’s follow tcp stream.

<img src="https://github.com/CSBCTF/IWDCTF/blob/a1af7520b6351d0c60d4149982ab76a74b47943c/Network/Plain%20Sight%203/files/3.1.png">
Here we can see the form login used by attackers to steal credentials from the victim and domain name of accounts.google.com is used!  IWDCTF{accounts.google.com}
