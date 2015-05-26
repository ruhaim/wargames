# level12 -> level13


[http://http://overthewire.org/wargames/bandit/bandit13.html](http://http://overthewire.org/wargames/bandit/bandit13.html)

-

    ssh bandit12@bandit.labs.overthewire.org

-

    bandit12@bandit.labs.overthewire.org's password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

-

    bandit9@melinda:~$ ls
    data.txt

-

    bandit12@melinda:/$ cd /tmp
    
-

    bandit12@melinda:/tmp$ mkdir sliitwar

-

    bandit12@melinda:/tmp~$ cd sliitwar

-

    bandit12@melinda:/tmp/sliitwar$ xxd -r ~/data.txt > data.txt

-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt
    
-
    
    bandit12@melinda:/tmp/sliitwar$ file data.txt
    data.txt: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression

-

    bandit12@melinda:/tmp/sliitwar$ zcat data.txt > dataNew

-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  dataNew

-

    bandit12@melinda:/tmp/sliitwar$ file dataNew
    dataNew: bzip2 compressed data, block size = 900k


-

    bandit12@melinda:/tmp/sliitwar$ bzip2 -d dataNew bzip-decompress
    bzip2: Can't guess original name for dataNew -- using dataNew.out

-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  dataNew.out

-

    bandit12@melinda:/tmp/sliitwar$ file dataNew.out
    dataNew.out: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression

-

    bandit12@melinda:/tmp/sliitwar$ zcat dataNew.out > moreNew
    
-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  dataNew.out  moreNew

-

    bandit12@melinda:/tmp/sliitwar$ file moreNew
    moreNew: POSIX tar archive (GNU)

-

    bandit12@melinda:/tmp/sliitwar$ tar -xvf moreNew
    data5.bin

-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  data5.bin  dataNew.out  moreNew
    
-

    bandit12@melinda:/tmp/sliitwar$ file data5.bin
    data5.bin: POSIX tar archive (GNU)

-

    bandit12@melinda:/tmp/sliitwar$ tar -xvf data5.bin
    data6.bin

-

    bandit12@melinda:/tmp/sliitwar$ file data6.bin
    data6.bin: bzip2 compressed data, block size = 900k

-

    
    bandit12@melinda:/tmp/sliitwar$ bunzip2 data6.bin
    bunzip2: Can't guess original name for data6.bin -- using data6.bin.out

-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  data5.bin  data6.bin.out  dataNew.out  moreNew
    
-

    bandit12@melinda:/tmp/sliitwar$ file data6.bin.out
    data6.bin.out: POSIX tar archive (GNU)

-

    bandit12@melinda:/tmp/sliitwar$ tar -xvf data6.bin.out
    data8.bin

-

    bandit12@melinda:/tmp/sliitwar$ file data8.bin
    data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression

-

    bandit12@melinda:/tmp/sliitwar$ zcat data8.bin > data8.out
    
-

    bandit12@melinda:/tmp/sliitwar$ ls
    data.txt  data5.bin  data6.bin.out  data8.bin  data8.out  dataNew.out  moreNew

-

    bandit12@melinda:/tmp/sliitwar$ file data8.out
    data8.out: ASCII text

-

    bandit12@melinda:/tmp/sliitwar$ cat data8.out
    The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
-
![](http://i.imgur.com/cbBBHrA.png)

![](http://i.imgur.com/M7AU67W.png)

![](http://i.imgur.com/FSo9z9d.png)

![](http://i.imgur.com/3iukc1g.png)






    










