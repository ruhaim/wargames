# level16 -> level17


[http://http://overthewire.org/wargames/bandit/bandit17.html](http://http://overthewire.org/wargames/bandit/bandit17.html)

-

    ssh bandit16@bandit.labs.overthewire.org

-

    bandit16@bandit.labs.overthewire.org's password: cluFn7wTiGryunymYOu4RcffSxQluehd

-

    bandit16@melinda:~$ nmap -p 31000-32000  localhost

-

    Starting Nmap 6.40 ( http://nmap.org ) at 2015-05-26 13:41 UTC
    Nmap scan report for localhost (127.0.0.1)
    Host is up (0.00078s latency).
    Not shown: 996 closed ports
    PORT  STATE SERVICE
    31046/tcp open  unknown
    31518/tcp open  unknown
    31691/tcp open  unknown
    31790/tcp open  unknown
    31960/tcp open  unknown
    
    Nmap done: 1 IP address (1 host up) scanned in 0.08 seconds

-

    bandit16@melinda:~$ openssl s_client -quiet -connect localhost:31046

-
    
    140737354045088:error:140770FC:SSL routines:SSL23_GET_SERVER_HELLO:unknown protocol:s23_clnt.c:795:

-

    bandit16@melinda:~$ openssl s_client -quiet -connect localhost:31518

-


    depth=0 CN = li190-250.members.linode.com
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = li190-250.members.linode.com
    verify return:1
    cluFn7wTiGryunymYOu4RcffSxQluehd

-

    cluFn7wTiGryunymYOu4RcffSxQluehd

-

    
    bandit16@melinda:~$ openssl s_client -quiet -connect localhost:31691

-


    140737354045088:error:140770FC:SSL routines:SSL23_GET_SERVER_HELLO:unknown protocol:s23_clnt.c:795:

-

    bandit16@melinda:~$ openssl s_client -quiet -connect localhost:31790
    
    
    depth=0 CN = li190-250.members.linode.com
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = li190-250.members.linode.com
    verify return:1

-

    cluFn7wTiGryunymYOu4RcffSxQluehd

-

    Correct!
    -----BEGIN RSA PRIVATE KEY-----
    MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
    imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
    Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
    DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
    JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
    x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
    KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
    J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
    d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
    YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
    vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
    +TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
    8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
    SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
    HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
    SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
    R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
    Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
    R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
    L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
    blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
    YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
    77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
    dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
    vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
    -----END RSA PRIVATE KEY-----
    
    read:errno=0

-

Copy the RSA Key to Clipboard

-

    bandit16@melinda:~$ mkdir /tmp/sliitwar2

-

    bandit16@melinda:~$ cd /tmp/sliitwar2

-

    bandit16@melinda:/tmp/sliitwar2$ openssl s_client -quiet -connect localhost:31790 > a.txt

-

    depth=0 CN = li190-250.members.linode.com
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = li190-250.members.linode.com
    verify return:1
    
-

    cluFn7wTiGryunymYOu4RcffSxQluehd
    read:errno=0

-

    bandit16@melinda:/tmp/sliitwar2$ ls
    a.txt  sshkey16.private

-

    bandit16@melinda:/tmp/sliitwar2$ nano a.txt


-

    Correct!
    -----BEGIN RSA PRIVATE KEY-----
    MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
    imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
    Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
    DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
    JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
    x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
    KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
    J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
    d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
    YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
    vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
    +TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
    8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
    SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
    HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
    SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
    R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
    Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
    R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
    L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
    blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
    YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
    77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
    dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
    vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
    -----END RSA PRIVATE KEY-----
    
    
    
    
    
    
    
    
    
    
    
    
    [ Read 29 lines ]
    ^G Get Help ^O WriteOut ^R Read File^Y Prev Page^K Cut Text ^C Cur Pos
    ^X Exit ^J Justify  ^W Where Is ^V Next Page^U UnCut Text   ^T To Spell
    
Remove the `Correct!` text from top of the file and exit, remember to Save before exit. To Exit Use `Ctrl + X`

-

    bandit16@melinda:/tmp/sliitwar2$ ls -a -l

-


    total 1104
    drwxrwxr-x2 bandit16 bandit164096 May 27 08:57 .
    drwxrwx-wt 4449 root root 1118208 May 27 09:13 ..
    -rw-rw-r--1 bandit16 bandit161676 May 27 09:04 a.txt
    -rw-rw-r--1 bandit16 bandit16   0 May 27 08:36 sshkey16.private

-

    bandit16@melinda:/tmp/sliitwar2$ chmod 700 a.txt

-

    bandit16@melinda:/tmp/sliitwar2$ ls -a -l

-

    total 1104
    drwxrwxr-x2 bandit16 bandit164096 May 27 08:57 .
    drwxrwx-wt 4449 root root 1118208 May 27 09:14 ..
    -rwx------1 bandit16 bandit161676 May 27 09:04 a.txt
    -rw-rw-r--1 bandit16 bandit16   0 May 27 08:36 sshkey16.private

-
    
    bandit16@melinda:/tmp/sliitwar2$ ssh -i a.txt bandit17@localhost
    
-

    Could not create directory '/home/bandit16/.ssh'.
    The authenticity of host 'localhost (127.0.0.1)' can't be established.
    ECDSA key fingerprint is 05:3a:1c:25:35:0a:ed:2f:cd:87:1c:f6:fe:69:e4:f6.
    Are you sure you want to continue connecting (yes/no)? 

-

    yes

-

    Failed to add the host to the list of known hosts (/home/bandit16/.ssh/known_hosts).

- 

    bandit17@melinda:~$



-

![](http://i.imgur.com/FrKxr6x.png)

![](http://i.imgur.com/gUXai5l.png)

![](http://i.imgur.com/y56ddJY.png)

![](http://i.imgur.com/IoQLGJE.png)

![](http://i.imgur.com/WpNLmLu.png)

![](http://i.imgur.com/d9GvZNH.png)
    