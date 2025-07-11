---
id: ssh-help
aliases:
  - ssh manual
tags: []
---

# SSH Manual Page

NAME
       ssh — OpenSSH remote login client

SYNOPSIS
       ssh   [-46AaCfGgKkMNnqsTtVvXxYy]   [-B   bind_interface]  [-b  bind_address]  [-c  cipher_spec]  [-D  [bind_address:]port]  [-E  log_file]
           [-e escape_char] [-F configfile] [-I  pkcs11]  [-i  identity_file]  [-J  destination]  [-L  address]  [-l  login_name]  [-m  mac_spec]
           [-O  ctl_cmd]  [-o  option]  [-P  tag]  [-p  port]  [-R  address] [-S ctl_path] [-W host:port] [-w local_tun[:remote_tun]] destination
           [command [argument ...]]
       ssh [-Q query_option]

DESCRIPTION
       ssh (SSH client) is a program for logging into a remote machine and for executing commands on a remote machine.  It is intended to provide
       secure encrypted communications between two untrusted  hosts  over  an  insecure  network.   X11  connections,  arbitrary  TCP  ports  and
       Unix-domain sockets can also be forwarded over the secure channel.

       ssh  connects  and  logs  into  the  specified  destination,  which  may  be  specified  as  either  [user@]hostname  or a URI of the form
       ssh://[user@]hostname[:port].  The user must prove their identity to the remote machine using one of several methods (see below).

       If a command is specified, it will be executed on the remote host instead of a login shell.  A complete command line may be  specified  as
       command,  or it may have additional arguments.  If supplied, the arguments will be appended to the command, separated by spaces, before it
       is sent to the server to be executed.

       The options are as follows:

       -4      Forces ssh to use IPv4 addresses only.

       -6      Forces ssh to use IPv6 addresses only.


