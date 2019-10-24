# SSH
## Secure Shell 
Hin örugga skel

---
<img src="https://i.imgur.com/cf3iAjN.png" width="550">
---
<img src="https://i.imgur.com/PG4VH2J.png" width="600">
---
```
OpenSSH_8.0p1, OpenSSL 1.0.2t  10 Sep 2019
debug1: Reading configuration data /etc/ssh/ssh_config
debug1: Connecting to hekla.rhi.hi.is [130.208.165.2] port 22.
debug1: Connection established.
debug1: identity file /home/teytur/.ssh/id_rsa type 0
debug1: identity file /home/teytur/.ssh/id_rsa-cert type -1
debug1: identity file /home/teytur/.ssh/id_dsa type -1
debug1: identity file /home/teytur/.ssh/id_dsa-cert type -1
debug1: identity file /home/teytur/.ssh/id_ecdsa type -1
debug1: identity file /home/teytur/.ssh/id_ecdsa-cert type -1
debug1: identity file /home/teytur/.ssh/id_ed25519 type -1
debug1: identity file /home/teytur/.ssh/id_ed25519-cert type -1
debug1: identity file /home/teytur/.ssh/id_xmss type -1
debug1: identity file /home/teytur/.ssh/id_xmss-cert type -1
debug1: Local version string SSH-2.0-OpenSSH_8.0
debug1: Remote protocol version 2.0, remote software version OpenSSH_5.3
debug1: match: OpenSSH_5.3 pat OpenSSH_5* compat 0x0c000002
debug1: Authenticating to hekla.rhi.hi.is:22 as 'teg6'
debug1: SSH2_MSG_KEXINIT sent
debug1: SSH2_MSG_KEXINIT received
debug1: kex: algorithm: diffie-hellman-group-exchange-sha256
debug1: kex: host key algorithm: ssh-rsa
debug1: kex: server->client cipher: aes128-ctr MAC: umac-64@openssh.com compression: none
debug1: kex: client->server cipher: aes128-ctr MAC: umac-64@openssh.com compression: none
debug1: SSH2_MSG_KEX_DH_GEX_REQUEST(2048<3072<8192) sent
debug1: got SSH2_MSG_KEX_DH_GEX_GROUP
debug1: SSH2_MSG_KEX_DH_GEX_INIT sent
debug1: got SSH2_MSG_KEX_DH_GEX_REPLY
debug1: Server host key: ssh-rsa SHA256:4jlEv000KCUwqreId0hqmCsGyQljTGO1qWnWC20TdGs
debug1: Host 'hekla.rhi.hi.is' is known and matches the RSA host key.
debug1: Found key in /home/teytur/.ssh/known_hosts:5
debug1: rekey out after 4294967296 blocks
debug1: SSH2_MSG_NEWKEYS sent
debug1: expecting SSH2_MSG_NEWKEYS
debug1: SSH2_MSG_NEWKEYS received
debug1: rekey in after 4294967296 blocks
debug1: Will attempt key: /home/teytur/.ssh/id_rsa RSA SHA256:Sv9fy0mW9SO7LxWqe5mr8UxSzx2jT6qo2zci7vAo1I8 agent
debug1: Will attempt key: /home/teytur/.ssh/id_dsa 
debug1: Will attempt key: /home/teytur/.ssh/id_ecdsa 
debug1: Will attempt key: /home/teytur/.ssh/id_ed25519 
debug1: Will attempt key: /home/teytur/.ssh/id_xmss 
debug1: SSH2_MSG_SERVICE_ACCEPT received
debug1: Authentications that can continue: publickey,gssapi-keyex,gssapi-with-mic,password
debug1: Next authentication method: publickey
debug1: Offering public key: /home/teytur/.ssh/id_rsa RSA SHA256:Sv9fy0mW9SO7LxWqe5mr8UxSzx2jT6qo2zci7vAo1I8 agent
debug1: Authentications that can continue: publickey,gssapi-keyex,gssapi-with-mic,password
debug1: Trying private key: /home/teytur/.ssh/id_dsa
debug1: Trying private key: /home/teytur/.ssh/id_ecdsa
debug1: Trying private key: /home/teytur/.ssh/id_ed25519
debug1: Trying private key: /home/teytur/.ssh/id_xmss
debug1: Next authentication method: password
teg6@hekla.rhi.hi.is's password: 
debug1: Authentication succeeded (password).
Authenticated to hekla.rhi.hi.is ([130.208.165.2]:22).
debug1: channel 0: new [client-session]
debug1: Requesting no-more-sessions@openssh.com
debug1: Entering interactive session.
debug1: pledge: network
Last login: Wed Oct 23 22:29:41 2019 from l46a-510.gardur.hi.is
+------------------------------------------------------------------------------+
|                                                                              |
|       Thu ert ad tengjast Heklu (hekla.rhi.hi.is) fjolnotendavel RHI.        |
|       Fyrir alla nemendur og starfsmenn Haskola Islands.                     |
|       Leidbeiningar: http://rhi.hi.is/fjolnotendatolvur                      |
|                                                                              |
|       You are connecting Hekla (hekla.rhi.hi.is) for all students and        |
|       staff of the University of Iceland.                                    |
|       Instructions: http://rhi.hi.is/multi_user_computers                    |
|                                                                              |
+------------------------------------------------------------------------------+

Styrikerfi: GNU/Linux
CentOS release 6.10 (Final)

Fjoldi tengdra notenda: 9
-bash-4.1$ 

```
---
