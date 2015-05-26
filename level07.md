# level6 -> level7


[http://http://overthewire.org/wargames/bandit/bandit7.html](http://http://overthewire.org/wargames/bandit/bandit7.html)

-

    ssh bandit6@bandit.labs.overthewire.org

-

    bandit6@bandit.labs.overthewire.org's password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7

-

    bandit6@melinda:~$ find / -size 33c -user bandit7 -group bandit6 -type f 2>/dev/null
    /var/lib/dpkg/info/bandit7.password

-

[http://askubuntu.com/questions/350208/what-does-2-dev-null-mean](http://askubuntu.com/questions/350208/what-does-2-dev-null-mean)

-

    bandit6@melinda:~$ cat /var/lib/dpkg/info/bandit7.password
    HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

-

![](http://i.imgur.com/dPOBJIT.png)

