# level19 -> level20


[http://http://overthewire.org/wargames/bandit/bandit20.html](http://http://overthewire.org/wargames/bandit/bandit20.html)

-

    ssh bandit19@bandit.labs.overthewire.org

-

    bandit19@bandit.labs.overthewire.org's password: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x


-

    bandit19@melinda:~$ ./bandit20-do

-

    Run a command as another user.
      Example: ./bandit20-do id

-

    bandit19@melinda:~$ ./bandit20-do id

-

    uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11020(bandit20),11019(bandit19)

-

    bandit19@melinda:~$ ./bandit20-do whoami

-

    bandit20

-

    bandit19@melinda:~$ whoami

-

    bandit19

-

    bandit19@melinda:~$ ./bandit20-do ls /etc/bandit_pass -l -a

-

    total 116
    drwxr-xr-x   2 root root 4096 May  3 12:32 .
    drwxr-xr-x 108 root root 4096 May 26 23:24 ..
    -r--------   1 bandit0  bandit0 8 Nov 14  2014 bandit0
    -r--------   1 bandit1  bandit133 Nov 14  2014 bandit1
    -r--------   1 bandit10 bandit10   33 Nov 14  2014 bandit10
    -r--------   1 bandit11 bandit11   33 Nov 14  2014 bandit11
    -r--------   1 bandit12 bandit12   33 Nov 14  2014 bandit12
    -r--------   1 bandit13 bandit13   33 Nov 14  2014 bandit13
    -r--------   1 bandit14 bandit14   33 Nov 14  2014 bandit14
    -r--------   1 bandit15 bandit15   33 Nov 14  2014 bandit15
    -r--------   1 bandit16 bandit16   33 Nov 14  2014 bandit16
    -r--------   1 bandit17 bandit17   33 Nov 14  2014 bandit17
    -r--------   1 bandit18 bandit18   33 Nov 14  2014 bandit18
    -r--------   1 bandit19 bandit19   33 Nov 14  2014 bandit19
    -r--------   1 bandit2  bandit233 Nov 14  2014 bandit2
    -r--------   1 bandit20 bandit20   33 Nov 14  2014 bandit20
    -r--------   1 bandit21 bandit21   33 Nov 14  2014 bandit21
    -r--------   1 bandit22 bandit22   33 Nov 14  2014 bandit22
    -r--------   1 bandit23 bandit23   33 Nov 14  2014 bandit23
    -r--------   1 bandit24 bandit24   33 May  3 12:32 bandit24
    -r--------   1 bandit25 bandit25   33 Nov 16  2014 bandit25
    -r--------   1 bandit26 bandit26   33 Nov 16  2014 bandit26
    -r--------   1 bandit3  bandit333 Nov 14  2014 bandit3
    -r--------   1 bandit4  bandit433 Nov 14  2014 bandit4
    -r--------   1 bandit5  bandit533 Nov 14  2014 bandit5
    -r--------   1 bandit6  bandit633 Nov 14  2014 bandit6
    -r--------   1 bandit7  bandit733 Nov 14  2014 bandit7
    -r--------   1 bandit8  bandit833 Nov 14  2014 bandit8
    -r--------   1 bandit9  bandit933 Nov 14  2014 bandit9

-

    bandit19@melinda:~$ ./bandit20-do cat /etc/bandit_pass/
    bandit20

-

    GbKksEFF4yrVs6il55v6gwY5aVje5f0j


-

![](http://i.imgur.com/Jxyfhfv.png)