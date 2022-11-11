# bashcat
a plain text chat via TCP, with support for multiple clients using netcat and socat

Note:
-
this is just for testing purposes, please do not use this in a serious setting, as every message is transferred in plain text.

Dependencies:
-

openbsd-netcat socat

Ussage:
-

git clone https://github.com/Tina-lel/bashcat && cd bashcat


**server setup:**

cd server

chmod +x server config

forward TCP ports if you want clients from outside of your network to connect (default ones are: 6868 and 6869,  you can change them in the config file)

touch main

./server


**client setup:**

cd client

chmod +x client config

open up the "config" file in a text editor and enter a hostname/ip address of a Machine running the "server" script and change your name.

./client

press ctrl+c to open the message box (the "newmsg:" text is a bit delayed, this is normal, you can type before it appears.)

you might need to type "!refresh" in order to see all messages

message box commands:
-

!refresh

!exit
