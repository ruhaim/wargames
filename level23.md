# level22 -> level23


[http://http://overthewire.org/wargames/bandit/bandit23.html](http://http://overthewire.org/wargames/bandit/bandit23.html)



-

    ssh bandit22@bandit.labs.overthewire.org

-

    bandit22@bandit.labs.overthewire.org's password: Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI

-

    bandit22@melinda:~$ cd /etc/cron.d

-

    bandit22@melinda:/etc/cron.d$ ls -al

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

    bandit22@melinda:/etc/cron.d$ cat cronjob_bandit23
    * * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null

-

    bandit22@melinda:/etc/cron.d$ cat /usr/bin/cronjob_bandit23.sh

-

    #!/bin/bash
    
    myname=$(whoami)
    mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
    
    echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"
    
    cat /etc/bandit_pass/$myname > /tmp/$mytarget

-

    bandit22@melinda:/etc/cron.d$ echo I am user bandit23 | md5sum | cut -d ' ' -f 1

-

    8ca319486bfbbc3663ea0fbe81326349

-

    bandit22@melinda:/etc/cron.d$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349

-

    jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n


-

![](http://i.imgur.com/ZsiIZpb.png)


    
       