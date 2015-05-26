# level13 -> level14


[http://http://overthewire.org/wargames/bandit/bandit14.html](http://http://overthewire.org/wargames/bandit/bandit14.html)

-

    ssh bandit13@bandit.labs.overthewire.org

-

    bandit13@bandit.labs.overthewire.org's password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

-
    
    bandit13@melinda:~$ ls
    sshkey.private

-

    bandit13@melinda:~$ ssh -i sshkey.private bandit14@localhost
    Could not create directory '/home/bandit13/.ssh'.
    The authenticity of host 'localhost (127.0.0.1)' can't be established.
    ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.


-

    Are you sure you want to continue connecting (yes/no)? yes
    Failed to add the host to the list of known hosts (/home/bandit13/.ssh/known_hosts).

-

    bandit14@melinda:/etc$ cd /etc/bandit_pass

-

    bandit14@melinda:/etc/bandit_pass$ cat bandit14
    4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

-

![](http://i.imgur.com/LE8N5LA.png)

![](http://i.imgur.com/LRwrjCp.png)
