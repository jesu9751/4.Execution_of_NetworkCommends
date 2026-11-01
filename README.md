# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output
```
1.C:\Users\acer>ipconfig

Windows IP Configuration


Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 3:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 4:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : 2405:201:e006:c15f:f7d5:82e:ebf:b911
   Temporary IPv6 Address. . . . . . : 2405:201:e006:c15f:c5d8:f6bb:4910:6c1e
   Link-local IPv6 Address . . . . . : fe80::5924:bf3d:75b7:d4f9%12
   IPv4 Address. . . . . . . . . . . : 192.168.29.85
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : fe80::8ea3:99ff:fec7:9e76%12
                                       192.168.29.1

Ethernet adapter Bluetooth Network Connection:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

2.C:\Users\acer>ping google.com

Pinging google.com [2404:6800:4002:817::200e] with 32 bytes of data:
Reply from 2404:6800:4002:817::200e: time=45ms
Reply from 2404:6800:4002:817::200e: time=53ms
Reply from 2404:6800:4002:817::200e: time=42ms
Reply from 2404:6800:4002:817::200e: time=40ms

Ping statistics for 2404:6800:4002:817::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 40ms, Maximum = 53ms, Average = 45ms

3.C:\Users\acer>tracert google.com

Tracing route to google.com [2404:6800:4002:817::200e]
over a maximum of 30 hops:

  1     1 ms     2 ms     3 ms  2405:201:e006:c15f:8ea3:99ff:fec7:9e76
  2     *        *        *     Request timed out.
  3     *        *        *     Request timed out.
  4     *        *        *     Request timed out.
  5    17 ms     9 ms     8 ms  2405:200:80c:3168:61::7
  6     *        *        *     Request timed out.
  7     *        4 ms     4 ms  2405:200:801:900::1296
  8     *        *        *     Request timed out.
  9    43 ms    44 ms    46 ms  tzdelb-bf-in-x0e.1e100.net [2404:6800:4002:817::200e]

Trace complete.

4.C:\Users\acer>nslookup wikipedia.org
Server:  reliance.reliance
Address:  2405:201:e006:c15f::c0a8:1d01

Non-authoritative answer:
Name:    wikipedia.org
Addresses:  2001:df2:e500:ed1a::1
          103.102.166.224


5.C:\Users\acer>netstat -ano

Active Connections

  Proto  Local Address          Foreign Address        State           PID
  TCP    0.0.0.0:80             0.0.0.0:0              LISTENING       4
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING       2024
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING       4
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING       2584
  TCP    0.0.0.0:7680           0.0.0.0:0              LISTENING       3056
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING       1720
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING       1548
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING       2296
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING       3452
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING       4528
  TCP    0.0.0.0:49672          0.0.0.0:0              LISTENING       1664
  TCP    0.0.0.0:56922          0.0.0.0:0              LISTENING       9520
  TCP    0.0.0.0:58995          0.0.0.0:0              LISTENING       4912
  TCP    127.0.0.1:4343         0.0.0.0:0              LISTENING       4880
  TCP    127.0.0.1:4449         0.0.0.0:0              LISTENING       4888
  TCP    127.0.0.1:5141         0.0.0.0:0              LISTENING       4936
  TCP    127.0.0.1:5141         127.0.0.1:64292        ESTABLISHED     4936
  TCP    127.0.0.1:15152        0.0.0.0:0              LISTENING       7272
  TCP    127.0.0.1:19443        0.0.0.0:0              LISTENING       5004
  TCP    127.0.0.1:28385        0.0.0.0:0              LISTENING       4
  TCP    127.0.0.1:28390        0.0.0.0:0              LISTENING       4
  TCP    127.0.0.1:46753        0.0.0.0:0              LISTENING       9824
  TCP    127.0.0.1:46760        0.0.0.0:0              LISTENING       9824
  TCP    127.0.0.1:46934        0.0.0.0:0              LISTENING       11312
  TCP    127.0.0.1:46935        0.0.0.0:0              LISTENING       11312
  TCP    127.0.0.1:46935        127.0.0.1:49773        ESTABLISHED     11312
  TCP    127.0.0.1:46936        0.0.0.0:0              LISTENING       6500
  TCP    127.0.0.1:46936        127.0.0.1:49762        ESTABLISHED     6500
  TCP    127.0.0.1:46937        0.0.0.0:0              LISTENING       6500
  TCP    127.0.0.1:46937        127.0.0.1:49765        ESTABLISHED     6500
  TCP    127.0.0.1:49350        0.0.0.0:0              LISTENING       4636
  TCP    127.0.0.1:49351        0.0.0.0:0              LISTENING       3076
  TCP    127.0.0.1:49669        127.0.0.1:49670        ESTABLISHED     4896
  TCP    127.0.0.1:49670        127.0.0.1:49669        ESTABLISHED     4896
  TCP    127.0.0.1:49675        127.0.0.1:49676        ESTABLISHED     9824
  TCP    127.0.0.1:49676        127.0.0.1:49675        ESTABLISHED     9824
  TCP    127.0.0.1:49717        127.0.0.1:58995        ESTABLISHED     5240
  TCP    127.0.0.1:49755        127.0.0.1:49756        ESTABLISHED     6500
  TCP    127.0.0.1:49756        127.0.0.1:49755        ESTABLISHED     6500
  TCP    127.0.0.1:49757        127.0.0.1:49758        ESTABLISHED     6500
  TCP    127.0.0.1:49758        127.0.0.1:49757        ESTABLISHED     6500
  TCP    127.0.0.1:49760        127.0.0.1:49761        ESTABLISHED     10124
  TCP    127.0.0.1:49761        127.0.0.1:49760        ESTABLISHED     10124
  TCP    127.0.0.1:49762        127.0.0.1:46936        ESTABLISHED     10124
  TCP    127.0.0.1:49763        127.0.0.1:49764        ESTABLISHED     10124
  TCP    127.0.0.1:49764        127.0.0.1:49763        ESTABLISHED     10124
  TCP    127.0.0.1:49765        127.0.0.1:46937        ESTABLISHED     10124
  TCP    127.0.0.1:49767        127.0.0.1:49768        ESTABLISHED     11312
  TCP    127.0.0.1:49768        127.0.0.1:49767        ESTABLISHED     11312
  TCP    127.0.0.1:49769        127.0.0.1:49770        ESTABLISHED     11312
  TCP    127.0.0.1:49770        127.0.0.1:49769        ESTABLISHED     11312
  TCP    127.0.0.1:49771        127.0.0.1:49772        ESTABLISHED     11272
  TCP    127.0.0.1:49772        127.0.0.1:49771        ESTABLISHED     11272
  TCP    127.0.0.1:49773        127.0.0.1:46935        ESTABLISHED     11272
  TCP    127.0.0.1:49811        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:49812        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:49814        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:49815        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:49816        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:49817        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50399        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50400        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50401        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50402        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50403        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50404        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50405        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50406        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50407        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50408        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50409        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:50410        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:51779        0.0.0.0:0              LISTENING       4896
  TCP    127.0.0.1:51780        0.0.0.0:0              LISTENING       4896
  TCP    127.0.0.1:51781        0.0.0.0:0              LISTENING       4896
  TCP    127.0.0.1:51782        0.0.0.0:0              LISTENING       4896
  TCP    127.0.0.1:53165        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:53166        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:53167        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:53168        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58933        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58934        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58935        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58936        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58937        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58938        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58939        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58940        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:58995        127.0.0.1:49717        ESTABLISHED     4912
  TCP    127.0.0.1:62348        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62349        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62350        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62352        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62355        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62356        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62358        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62359        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62360        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62361        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62362        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62363        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62364        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62365        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62548        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62549        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:62550        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63173        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63175        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63176        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63179        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63180        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63181        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63182        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:63183        127.0.0.1:49350        TIME_WAIT       0
  TCP    127.0.0.1:64292        127.0.0.1:5141         ESTABLISHED     11532
  TCP    192.168.29.85:139      0.0.0.0:0              LISTENING       4
  TCP    192.168.29.85:51396    172.64.148.235:443     ESTABLISHED     6700
  TCP    192.168.29.85:56950    31.7.60.154:85         ESTABLISHED     14672
  TCP    192.168.29.85:58942    20.247.162.75:443      ESTABLISHED     11780
  TCP    192.168.29.85:62357    20.184.175.23:443      ESTABLISHED     5512
  TCP    192.168.29.85:62545    20.190.145.142:443     ESTABLISHED     1252
  TCP    [::]:80                [::]:0                 LISTENING       4
  TCP    [::]:135               [::]:0                 LISTENING       2024
  TCP    [::]:445               [::]:0                 LISTENING       4
  TCP    [::]:7680              [::]:0                 LISTENING       3056
  TCP    [::]:49664             [::]:0                 LISTENING       1720
  TCP    [::]:49665             [::]:0                 LISTENING       1548
  TCP    [::]:49666             [::]:0                 LISTENING       2296
  TCP    [::]:49667             [::]:0                 LISTENING       3452
  TCP    [::]:49668             [::]:0                 LISTENING       4528
  TCP    [::]:49672             [::]:0                 LISTENING       1664
  TCP    [::]:58995             [::]:0                 LISTENING       4912
  TCP    [::1]:42050            [::]:0                 LISTENING       5100
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:49408  [2603:1040:a06:6::]:443  ESTABLISHED     5872
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:49810  [2405:200:1630:a03::312c:c5c9]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:49813  [2600:1901:1:7c5::]:443  ESTABLISHED     9520
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:49921  [2a03:2880:f369:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:50551  [2606:4700:9c62:7cbc:c23b:308:5ff2:75c4]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:51006  [2a03:2880:f315:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:51127  [2404:6800:4002:81a::200e]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:51516  [2404:6800:4013:807::64]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:52217  [2404:6800:4003:c1a::bc]:5228  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:52509  [2606:4700:83b1:d8b7:9afe:2d8:ccf5:ac50]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:52953  [2603:1020:5:1a::1c6]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:53164  [2a03:2880:f315:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:54157  [2a03:2880:f315:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:54556  [2a03:2880:f315:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:55607  [2001:4860:482b:7700::]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:56345  [2a03:2880:f335:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:56671  [2606:4700:83b1:d8b7:9afe:2d8:ccf5:ac50]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:57235  [2403:8600:c090:42:f000::1122]:443  CLOSE_WAIT      6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:58932  [2a03:2880:f315:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:58941  [2603:1061:14:151::1]:443  ESTABLISHED     11780
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:60208  [2a03:2880:f315:120:face:b00c:0:167]:443  ESTABLISHED     484
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62346  [2a03:2880:f369:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62347  [2606:4700:83b2:7cbc:c2c6:bf9:5ff2:75c4]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62351  [2606:4700:83b2:7cbc:c23b:de9:5ff2:75c4]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62353  [2a03:2880:f335:120:face:b00c:0:167]:443  ESTABLISHED     11780
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62354  [2600:14e1:18:6d::]:80  ESTABLISHED     11780
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62543  [2a03:2880:f335:120:face:b00c:0:167]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62546  [2603:1046:c06:c72::2]:443  ESTABLISHED     13044
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:62547  [2603:1046:c06:c72::2]:443  ESTABLISHED     13044
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:63170  [2620:1ec:33:1::11]:443  TIME_WAIT       0
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:63177  [2405:200:1630:a03::312c:c5ca]:80  ESTABLISHED     15924
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:63178  [2405:200:1630:a03::312c:c5ca]:80  ESTABLISHED     15924
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:63848  [2606:4700:83b2:7cbc:c23b:af8:5ff2:75c4]:443  ESTABLISHED     6700
  TCP    [2405:201:e006:c15f:c5d8:f6bb:4910:6c1e]:65256  [2a03:2880:f335:120:face:b00c:0:167]:443  TIME_WAIT       0
  UDP    0.0.0.0:123            *:*                                    15316
  UDP    0.0.0.0:5050           *:*                                    2584
  UDP    0.0.0.0:5353           *:*                                    14940
  UDP    0.0.0.0:5353           *:*                                    6700
  UDP    0.0.0.0:5353           *:*                                    14940
  UDP    0.0.0.0:5353           *:*                                    2304
  UDP    0.0.0.0:5353           *:*                                    6700
  UDP    0.0.0.0:5355           *:*                                    2304
  UDP    0.0.0.0:49259          0.0.32.14:443                          6700
  UDP    0.0.0.0:53350          *:*                                    2304
  UDP    0.0.0.0:56618          *:*                                    5240
  UDP    0.0.0.0:61177          *:*                                    2304
  UDP    127.0.0.1:1900         *:*                                    8484
  UDP    127.0.0.1:49664        127.0.0.1:49664                        4336
  UDP    127.0.0.1:52377        *:*                                    8484
  UDP    127.0.0.1:56617        *:*                                    5240
  UDP    192.168.29.85:137      *:*                                    4
  UDP    192.168.29.85:138      *:*                                    4
  UDP    192.168.29.85:1900     *:*                                    8484
  UDP    192.168.29.85:52376    *:*                                    8484
  UDP    [::]:123               *:*                                    15316
  UDP    [::]:5353              *:*                                    14940
  UDP    [::]:5353              *:*                                    6700
  UDP    [::]:5353              *:*                                    2304
  UDP    [::]:5355              *:*                                    2304
  UDP    [::]:49259             [2404:6800:4007:830::200e]:443                  6700
  UDP    [::]:53350             *:*                                    2304
  UDP    [::]:61177             *:*                                    2304
  UDP    [::1]:1900             *:*                                    8484
  UDP    [::1]:52375            *:*                                    8484
  UDP    [fe80::5924:bf3d:75b7:d4f9%12]:1900  *:*                                    8484
  UDP    [fe80::5924:bf3d:75b7:d4f9%12]:52374  *:*                                    8484

6.C:\Users\acer>arp -a

Interface: 192.168.29.85 --- 0xc
  Internet Address      Physical Address      Type
  192.168.29.1          8c-a3-99-c7-9e-76     dynamic
  192.168.29.176        10-2d-41-2d-8b-97     dynamic
  192.168.29.255        ff-ff-ff-ff-ff-ff     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static

7.C:\Users\acer>route print
===========================================================================
Interface List
 16...74 d4 dd cf 7d df ......Realtek PCIe GbE Family Controller
  9...fc 6d 77 8b 9d b9 ......Microsoft Wi-Fi Direct Virtual Adapter #3
 13...fe 6d 77 8b 9d b8 ......Microsoft Wi-Fi Direct Virtual Adapter #4
 12...fc 6d 77 8b 9d b8 ......Intel(R) Wi-Fi 6E AX211 160MHz
  1...........................Software Loopback Interface 1
===========================================================================

IPv4 Route Table
===========================================================================
Active Routes:
Network Destination        Netmask          Gateway       Interface  Metric
          0.0.0.0          0.0.0.0     192.168.29.1    192.168.29.85     50
        127.0.0.0        255.0.0.0         On-link         127.0.0.1    331
        127.0.0.1  255.255.255.255         On-link         127.0.0.1    331
  127.255.255.255  255.255.255.255         On-link         127.0.0.1    331
     192.168.29.0    255.255.255.0         On-link     192.168.29.85    306
    192.168.29.85  255.255.255.255         On-link     192.168.29.85    306
   192.168.29.255  255.255.255.255         On-link     192.168.29.85    306
        224.0.0.0        240.0.0.0         On-link         127.0.0.1    331
        224.0.0.0        240.0.0.0         On-link     192.168.29.85    306
  255.255.255.255  255.255.255.255         On-link         127.0.0.1    331
  255.255.255.255  255.255.255.255         On-link     192.168.29.85    306
===========================================================================
Persistent Routes:
  None

IPv6 Route Table
===========================================================================
Active Routes:
 If Metric Network Destination      Gateway
 12     66 ::/0                     fe80::8ea3:99ff:fec7:9e76
  1    331 ::1/128                  On-link
 12     66 2405:201:e006:c15f::/64  On-link
 12    306 2405:201:e006:c15f:c5d8:f6bb:4910:6c1e/128
                                    On-link
 12    306 2405:201:e006:c15f:f7d5:82e:ebf:b911/128
                                    On-link
 12    306 fe80::/64                On-link
 12    306 fe80::5924:bf3d:75b7:d4f9/128
                                    On-link
  1    331 ff00::/8                 On-link
 12    306 ff00::/8                 On-link
===========================================================================
Persistent Routes:
  None

8.C:\Users\acer>hostname
TMP215-75-G2

9.C:\Users\acer>getmac

Physical Address    Transport Name
=================== ==========================================================
74-D4-DD-CF-7D-DF   Media disconnected
FC-6D-77-8B-9D-B8   \Device\Tcpip_{7A6A847A-F6EB-45DC-9AF2-02E1723B3606}

10.C:\Users\acer>systeminfo

Host Name:                     TMP215-75-G2
OS Name:                       Microsoft Windows 11 Pro
OS Version:                    10.0.26300 N/A Build 26300
OS Manufacturer:               Microsoft Corporation
OS Configuration:              Standalone Workstation
OS Build Type:                 Multiprocessor Free
Registered Owner:              acer
Registered Organization:       N/A
Product ID:                    00330-80000-00000-AA830
Original Install Date:         15-10-2026, 18:46:59
System Boot Time:              30-10-2026, 08:16:54
System Manufacturer:           Acer
System Model:                  TravelMate P215-75-G2-TCO
System Type:                   x64-based PC
Processor(s):                  1 Processor(s) Installed.
                               [01]: Intel64 Family 6 Model 170 Stepping 4 GenuineIntel ~1200 Mhz
BIOS Version:                  INSYDE Corp. V1.05tt01a, 01-09-2025
Windows Directory:             C:\WINDOWS
System Directory:              C:\WINDOWS\system32
Boot Device:                   \Device\HarddiskVolume1
System Locale:                 en-us;English (United States)
Input Locale:                  00004009
Time Zone:                     (UTC+05:30) Chennai, Kolkata, Mumbai, New Delhi
Total Physical Memory:         15,869 MB
Available Physical Memory:     2,591 MB
Virtual Memory: Max Size:      19,581 MB
Virtual Memory: Available:     3,574 MB
Virtual Memory: In Use:        16,007 MB
Page File Location(s):         C:\pagefile.sys
Domain:                        WORKGROUP
Logon Server:                  \\TMP215-75-G2
Hotfix(s):                     4 Hotfix(s) Installed.
                               [01]: KB5127694
                               [02]: KB5121794
                               [03]: KB5127648
                               [04]: KB5127647
Network Card(s):               3 NIC(s) Installed.
                               [01]: Realtek PCIe GbE Family Controller
                                     Connection Name: Ethernet
                                     Status:          Media disconnected
                               [02]: Intel(R) Wi-Fi 6E AX211 160MHz
                                     Connection Name: Wi-Fi
                                     DHCP Enabled:    Yes
                                     DHCP Server:     192.168.29.1
                                     IP address(es)
                                     [01]: 192.168.29.85
                                     [02]: fe80::5924:bf3d:75b7:d4f9
                                     [03]: 2405:201:e006:c15f:b983:3da7:d237:159d
                                     [04]: 2405:201:e006:c15f:f7d5:82e:ebf:b911
                               [03]: Bluetooth Device (Personal Area Network)
                                     Connection Name: Bluetooth Network Connection
                                     Status:          Media disconnected
Virtualization-based security: Status: Running
                               Required Security Properties:
                                     Base Virtualization Support
                               Available Security Properties:
                                     Base Virtualization Support
                                     Secure Boot
                                     DMA Protection
                                     UEFI Code Readonly
                                     SMM Security Mitigations 1.0
                                     Mode Based Execution Control
                                     APIC Virtualization
                               Services Configured:
                                     Hypervisor enforced Code Integrity
                               Services Running:
                                     Hypervisor enforced Code Integrity
                               App Control for Business policy: Enforced
                               App Control for Business user mode policy: Off
                               Security Features Enabled:
Hyper-V Requirements:          A hypervisor has been detected. Features required for Hyper-V will not be displayed.
```

## Result
Thus Execution of Network commands Performed 
