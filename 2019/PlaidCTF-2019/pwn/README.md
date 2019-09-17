# Pwn

## SPlaid Birch

Pwnable (300 pts)
I make sure never to use
`scanf("%s")`
when doing competitive programming so that my solutions don't have buffer overflows. But writing algorithms is hard.

[files](https://play.plaidctf.com/files/splaid-birch_c4bb20002c1f46a8a360d3eba748af59.zip)

`splaid-birch.pwni.ng:17579`

## Spectre

Pwnable (666 pts)
Read the [flag](http://spectre.pwni.ng:4000/). Don't trust anything.

Download the [vm](https://play.plaidctf.com/files/spectre_161f05f267601806bdcd2c499fbf3930). Workers are running Ubuntu 18.04 on GCE with 1 vCPU and 1 GB of memory. 

## Suffarring

Pwnable (500 pts)
Some days I want to do string manipulation. And I want to do it fast! This guy is optimal up to log factors.

[files](https://play.plaidctf.com/files/suffarring_9617710f014cef44de2baac6219ff38d.zip)

`nc suffarring.pwni.ng 7361`

## Plaid Adventure II

Pwnable (250 pts)
Embark on another adventure! Restore from the savefile "flag.glksave" on the server to get the flag. (Apologies to Zarf for making a Glulx pwnable.) 

```
stty -icanon -echo

nc plaidadventure2.pwni.ng 6910

stty sane
```

[download](https://play.plaidctf.com/files/Plaid_Adventure_2_36c2f32fe0c0866eeb250b7ac2f48310.ulx)

## cppp

Pwnable (150 pts)
C++ is hard.

`cppp.pwni.ng 4444`

[binary](https://play.plaidctf.com/files/cppp_58fc210859e4c5e43d051b6476cbc9f7), [libc](https://play.plaidctf.com/files/libc-2.27_50390b2ae8aaa73c47745040f54e602f.so)

Hint: Additional port
The service is now also running on `cppp.pwni.ng:7777` for those ISPs that block egress to port `4444`.