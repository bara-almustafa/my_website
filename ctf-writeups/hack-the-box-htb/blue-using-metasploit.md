# Blue (using metasploit)

<figure><img src="../../.gitbook/assets/Blue.png" alt=""><figcaption></figcaption></figure>

firstly let\`s find open ports using nmap :

<figure><img src="../../.gitbook/assets/1.png" alt=""><figcaption></figcaption></figure>

so there is smb lets check its version using metasploit&#x20;

> using this commnad to open metasploit&#x20;

```
msfconsole
```

then lets search about smb version

> ![](../../.gitbook/assets/3.png)

use 103

<figure><img src="../../.gitbook/assets/4.png" alt=""><figcaption></figcaption></figure>

then lets enter options to see what does options we have&#x20;

we can see must enter the rhosts which its the target ip&#x20;

<figure><img src="../../.gitbook/assets/5.png" alt=""><figcaption></figcaption></figure>

as detatils we see windows 7 professional SP1  and SMB 1,2  as its details its eternalblue cve&#x20;

here is the some links of wanna some details of CVE-2017-0144

{% embed url="https://nvd.nist.gov/vuln/detail/cve-2017-0144" %}

{% embed url="https://cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2017-0144" %}

now lets search enternalblue in metasploit

<figure><img src="../../.gitbook/assets/6.png" alt=""><figcaption></figcaption></figure>

use 0

then enter the ip address of target in RHOSTS and in LPORT is tun0

<figure><img src="../../.gitbook/assets/7.png" alt=""><figcaption></figcaption></figure>

then run&#x20;

<figure><img src="../../.gitbook/assets/8.png" alt=""><figcaption></figcaption></figure>

here is we exploit it the machine&#x20;

and enter 'shell' to enter cmd shell enviroment&#x20;

<figure><img src="../../.gitbook/assets/9.png" alt=""><figcaption></figcaption></figure>

you will find the the user.txt in c:\Users\haris\Desktop\user.txt and root flag in c:\Users\Administrator\Desktop\root.txt

<figure><img src="../../.gitbook/assets/10.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/11.png" alt=""><figcaption></figcaption></figure>
