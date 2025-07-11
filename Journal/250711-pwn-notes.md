---
id: 250711-pwn-notes
aliases: []
tags: []
---

# User Privilege escalation 

log in into pwn-box with HTB provide log in for user1 
was able to escalate to user2 using: 

```bash 
sudo -l 
sudo -u user2 /bin/bash

```

flag.txt found /home/ dir - copy and pasted to hacking machine. 

## esciation to root 

- cd into the /root/ folder and located the id_rsa file 
- copied the if_rsa file to host machine and ran 

```bash 
chmod 600 id_rsa 
ssh root@{target.ip} -p {port} -i id_rsa
```

- flag located in home dir. 





