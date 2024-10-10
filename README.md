# peerchat-web
This is a web-rtc based video calling web application. It uses a third party platform, agora. It is built using html, css and js.
It allows us to make a peer to peer connection between two users to exchange audio and video without a server once the connection is made.

working
So, first we use agora's signaling api to send the SDP and ICE Candidates of user-1 over to user-2 in the form of an offer. User-2 responds by sending their SDP and ICE Candidates in form of an answer. These Ice candidates are being created using google's stun servers. Once the connection is made we no longer need a signaling server. The video and audio will be exchanged directly between the two users.

Note:
You don't specifically need agora. You can build your own signaling api from scratch. However, i have used it because its free and provides 10000 minutes of use.
