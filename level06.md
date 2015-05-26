# level5 -> level6

[http://http://overthewire.org/wargames/bandit/bandit6.html](http://http://overthewire.org/wargames/bandit/bandit6.html)

-

    ssh bandit5@bandit.labs.overthewire.org

-

    bandit5@bandit.labs.overthewire.org's password: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

-
[http://en.wikipedia.org/wiki/Find](http://en.wikipedia.org/wiki/Find)

[http://unixhelp.ed.ac.uk/CGI/man-cgi?find](http://unixhelp.ed.ac.uk/CGI/man-cgi?find)

[http://en.wikipedia.org/wiki/Du_(Unix)](http://en.wikipedia.org/wiki/Du_(Unix))

[http://unix.stackexchange.com/questions/43148/unix-commands-help-find](http://unix.stackexchange.com/questions/43148/unix-commands-help-find)

-

    bandit5@melinda:~$ ls
    inhere

-

    bandit5@melinda:~$ cd inhere/

-

    bandit5@melinda:~/inhere$ find . -size 1033c -type f
    ./maybehere07/.file2

-

    bandit5@melinda:~/inhere$ cat< maybehere07/.file2
    DXjZPULLxYr17uwoI01bNLQbtFemEgo7

-
![](http://i.imgur.com/5jmtsgU.png)




