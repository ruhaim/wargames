# level15 -> level16


[http://http://overthewire.org/wargames/bandit/bandit16.html](http://http://overthewire.org/wargames/bandit/bandit16.html)

-

    ssh bandit15@bandit.labs.overthewire.org

-

    bandit15@bandit.labs.overthewire.org's password: BfMYroe26WYalil77FoDi9qh59eK5xNr

-
    
    bandit15@melinda:~$ openssl s_client -connect localhost:30001

-

    CONNECTED(00000003)
    depth=0 CN = li190-250.members.linode.com
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = li190-250.members.linode.com
    verify return:1
    ---
    Certificate chain
     0 s:/CN=li190-250.members.linode.com
       i:/CN=li190-250.members.linode.com
    ---
    Server certificate
    -----BEGIN CERTIFICATE-----
    MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
    BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
    WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
    aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
    WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
    ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
    TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
    yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
    a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
    ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
    AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
    dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
    fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
    5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
    MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
    kDzwlmBO4WKSmCAuky44cXmd
    -----END CERTIFICATE-----
    subject=/CN=li190-250.members.linode.com
    issuer=/CN=li190-250.members.linode.com
    ---
    No client certificate CA names sent
    ---
    SSL handshake has read 1330 bytes and written 455 bytes
    ---
    New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA
    Server public key is 2048 bit
    Secure Renegotiation IS supported
    Compression: NONE
    Expansion: NONE
    SSL-Session:
    Protocol  : SSLv3
    Cipher: DHE-RSA-AES256-SHA
    Session-ID: F6A422D9FFF25A96295A1D20E2437D5194F7AB24C20939AA704FFE2BAEEA4F97
    Session-ID-ctx:
    Master-Key: FD946F8E085DF9B891416828478F6DE52E40608D300BA4F8DFC82C31EC03F5A4009ACCB5796410579733D19BF069451A
    Key-Arg   : None
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    Start Time: 1432646914
    Timeout   : 300 (sec)
    Verify return code: 18 (self signed certificate)
    ---

-

    BfMYroe26WYalil77FoDi9qh59eK5xNr

-

    HEARTBEATING
    read R BLOCK
    read:errno=0

-

    bandit15@melinda:~$ openssl s_client -quiet -connect localhost:30001

-

    depth=0 CN = li190-250.members.linode.com
    verify error:num=18:self signed certificate
    verify return:1
    depth=0 CN = li190-250.members.linode.com
    verify return:1

-

    BfMYroe26WYalil77FoDi9qh59eK5xNr

-

    Correct!
    cluFn7wTiGryunymYOu4RcffSxQluehd
    
    read:errno=0

-
![](http://i.imgur.com/WpE9xbM.png)

![](http://i.imgur.com/ei3YAZA.png)