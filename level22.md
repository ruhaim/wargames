# level21 -> level22


[http://http://overthewire.org/wargames/bandit/bandit22.html](http://http://overthewire.org/wargames/bandit/bandit22.html)



-

    ssh bandit21@bandit.labs.overthewire.org

-

    bandit21@bandit.labs.overthewire.org's password: gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr

-

    bandit21@melinda:~$ cd /etc/cron.d

-
    
    bandit21@melinda:/etc/cron.d$ ls -la

-

    total 100
    drwxr-xr-x   2 root root 4096 May  3 12:32 .
    drwxr-xr-x 108 root root 4096 May 27 11:11 ..
    -rw-r--r--   1 root root  102 Feb  9  2013 .placeholder
    -r--r-----   1 root root   46 Nov 14  2014 behemoth4_cleanup
    -rw-r--r--   1 root root  355 May 25  2013 cron-apt
    -rw-r--r--   1 root root   61 Nov 14  2014 cronjob_bandit22
    -rw-r--r--   1 root root   62 Nov 14  2014 cronjob_bandit23
    -rw-r--r--   1 root root   61 May  3 12:32 cronjob_bandit24
    -rw-r--r--   1 root root   62 May  3 12:32 cronjob_bandit24_root
    -r--r-----   1 root root   47 Nov 14  2014 leviathan5_cleanup
    -rw-------   1 root root  233 Nov 14  2014 manpage3_resetpw_job
    -rw-r--r--   1 root root   51 Nov 14  2014 melinda-stats
    -rw-r--r--   1 root root   54 Nov 14  2014 natas-session-toucher
    -rw-r--r--   1 root root   49 Nov 15  2014 natas-stats
    -r--r-----   1 root root   47 Nov 14  2014 natas25_cleanup
    -r--r-----   1 root root   47 Nov 14  2014 natas26_cleanup
    -r--r-----   1 root root   43 Nov 15  2014 natas27_cleanup
    -rw-r--r--   1 root root  510 Oct 29  2014 php5
    -rw-r--r--   1 root root   58 Nov 14  2014 semtex0-32
    -rw-r--r--   1 root root   58 Nov 14  2014 semtex0-64
    -rw-r--r--   1 root root   59 Nov 14  2014 semtex0-ppc
    -rw-r--r--   1 root root   35 Nov 14  2014 semtex5
    -rw-r--r--   1 root root  396 Nov 10  2013 sysstat
    -rw-r--r--   1 root root   29 Nov 14  2014 vortex0
    -rw-r--r--   1 root root   30 Nov 14  2014 vortex20

-

    bandit21@melinda:/etc/cron.d$ cat cronjob_bandit22
    * * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null

-

    bandit21@melinda:/etc/cron.d$ cat /usr/bin/cronjob_bandit22.sh

-

    #!/bin/bash
    chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
    cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

-

    bandit21@melinda:/etc/cron.d$ cat /etc/bandit_pass/bandit22

-

    cat: /etc/bandit_pass/bandit22: Permission denied

-

    bandit21@melinda:/etc/cron.d$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

-

    Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

-
![](http://i.imgur.com/aPxb0Hu.png)