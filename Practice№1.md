# Задание№1

cat /etc/passwd

root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
irc:x:39:39:ircd:/run/ircd:/usr/sbin/nologin
_apt:x:42:65534::/nonexistent:/usr/sbin/nologin
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
systemd-network:x:998:998:systemd Network Management:/:/usr/sbin/nologin
dhcpcd:x:996:996:DHCP Client Daemon:/usr/lib/dhcpcd:/bin/false
messagebus:x:995:995:System Message Bus:/nonexistent:/usr/sbin/nologin
syslog:x:100:101::/nonexistent:/usr/sbin/nologin
systemd-resolve:x:989:989:systemd Resolver:/:/usr/sbin/nologin
_chrony:x:988:988:Chrony Daemon:/var/lib/chrony:/usr/sbin/nologin
tss:x:987:987:tss user for tpm2:/:/usr/sbin/nologin
uuidd:x:101:105::/run/uuidd:/usr/sbin/nologin
systemd-oom:x:986:986:systemd Userspace OOM Killer:/:/usr/sbin/nologin
whoopsie:x:102:108::/nonexistent:/bin/false
dnsmasq:x:999:65534:dnsmasq:/var/lib/misc:/usr/sbin/nologin
avahi:x:103:109:Avahi mDNS daemon:/run/avahi-daemon:/usr/sbin/nologin
nm-openvpn:x:984:984:NetworkManager OpenVPN:/var/lib/openvpn/chroot:/usr/sbin/nologin
tcpdump:x:983:983:tcpdump:/nonexistent:/usr/sbin/nologin
sssd:x:104:110:SSSD system user:/var/lib/sss:/usr/sbin/nologin
speech-dispatcher:x:105:29:Speech Dispatcher:/run/speech-dispatcher:/bin/false
usbmux:x:106:46:usbmux daemon:/var/lib/usbmux:/usr/sbin/nologin
cups-pk-helper:x:107:111:user for cups-pk-helper service:/nonexistent:/usr/sbin/nologin
fwupd-refresh:x:982:982:Firmware update daemon:/var/lib/fwupd:/usr/sbin/nologin
saned:x:108:112::/var/lib/saned:/usr/sbin/nologin
geoclue:x:109:113::/var/lib/geoclue:/usr/sbin/nologin
cups-browsed:x:110:111::/nonexistent:/usr/sbin/nologin
pipewire:x:981:981:system user for pipewire:/nonexistent:/usr/sbin/nologin
hplip:x:111:7:HPLIP system user:/run/hplip:/bin/false
gnome-remote-desktop:x:980:980:GNOME Remote Desktop:/var/lib/gnome-remote-desktop:/usr/sbin/nologin
polkitd:x:979:979:User for polkitd:/:/usr/sbin/nologin
rtkit:x:978:978:RealtimeKit:/proc:/usr/sbin/nologin
colord:x:977:977:colord colour management daemon:/var/lib/colord:/usr/sbin/nologin
gdm:x:975:975:Gnome Display Manager:/var/lib/gdm3:/bin/false
elizaveta:x:1000:1000:elizaveta:/home/elizaveta:/bin/bash
vboxadd:x:997:1::/var/run/vboxadd:/bin/false

grep -o '^[a-zA-Z0-9_-]*' /etc/passwd | sort

_apt
avahi
backup
bin
_chrony
colord
cups-browsed
cups-pk-helper
daemon
dhcpcd
dnsmasq
elizaveta
fwupd-refresh
games
gdm
geoclue
gnome-remote-desktop
hplip
irc
list
lp
mail
man
messagebus
news
nm-openvpn
nobody
pipewire
polkitd
proxy
root
rtkit
saned
speech-dispatcher
sssd
sync
sys
syslog
systemd-network
systemd-oom
systemd-resolve
tcpdump
tss
usbmux
uucp
uuidd
vboxadd
whoopsie
www-data

# Задание№2

cat /etc/protocols

ip	0	IP		# internet protocol, pseudo protocol number
hopopt	0	HOPOPT		# IPv6 Hop-by-Hop Option [RFC1883]
icmp	1	ICMP		# internet control message protocol
igmp	2	IGMP		# Internet Group Management
ggp	3	GGP		# gateway-gateway protocol
ipencap	4	IP-ENCAP	# IP encapsulated in IP (officially ``IP'')
st	5	ST		# ST datagram mode
tcp	6	TCP		# transmission control protocol
egp	8	EGP		# exterior gateway protocol
igp	9	IGP		# any private interior gateway (Cisco)
pup	12	PUP		# PARC universal packet protocol
udp	17	UDP		# user datagram protocol
hmp	20	HMP		# host monitoring protocol
xns-idp	22	XNS-IDP		# Xerox NS IDP
rdp	27	RDP		# "reliable datagram" protocol
iso-tp4	29	ISO-TP4		# ISO Transport Protocol class 4 [RFC905]
dccp	33	DCCP		# Datagram Congestion Control Prot. [RFC4340]
xtp	36	XTP		# Xpress Transfer Protocol
ddp	37	DDP		# Datagram Delivery Protocol
idpr-cmtp 38	IDPR-CMTP	# IDPR Control Message Transport
ipv6	41	IPv6		# Internet Protocol, version 6
ipv6-route 43	IPv6-Route	# Routing Header for IPv6
ipv6-frag 44	IPv6-Frag	# Fragment Header for IPv6
idrp	45	IDRP		# Inter-Domain Routing Protocol
rsvp	46	RSVP		# Reservation Protocol
gre	47	GRE		# General Routing Encapsulation
esp	50	IPSEC-ESP	# Encap Security Payload [RFC2406]
ah	51	IPSEC-AH	# Authentication Header [RFC2402]
skip	57	SKIP		# SKIP
ipv6-icmp 58	IPv6-ICMP	# ICMP for IPv6
ipv6-nonxt 59	IPv6-NoNxt	# No Next Header for IPv6
ipv6-opts 60	IPv6-Opts	# Destination Options for IPv6
rspf	73	RSPF CPHB	# Radio Shortest Path First (officially CPHB)
vmtp	81	VMTP		# Versatile Message Transport
eigrp	88	EIGRP		# Enhanced Interior Routing Protocol (Cisco)
ospf	89	OSPFIGP		# Open Shortest Path First IGP
ax.25	93	AX.25		# AX.25 frames
ipip	94	IPIP		# IP-within-IP Encapsulation Protocol
etherip	97	ETHERIP		# Ethernet-within-IP Encapsulation [RFC3378]
encap	98	ENCAP		# Yet Another IP encapsulation [RFC1241]
#	99			# any private encryption scheme
pim	103	PIM		# Protocol Independent Multicast
ipcomp	108	IPCOMP		# IP Payload Compression Protocol
vrrp	112	VRRP		# Virtual Router Redundancy Protocol [RFC5798]
l2tp	115	L2TP		# Layer Two Tunneling Protocol [RFC2661]
isis	124	ISIS		# IS-IS over IPv4
sctp	132	SCTP		# Stream Control Transmission Protocol
fc	133	FC		# Fibre Channel
mobility-header 135 Mobility-Header # Mobility Support for IPv6 [RFC3775]
udplite	136	UDPLite		# UDP-Lite [RFC3828]
mpls-in-ip 137	MPLS-in-IP	# MPLS-in-IP [RFC4023]
manet	138			# MANET Protocols [RFC5498]
hip	139	HIP		# Host Identity Protocol
shim6	140	Shim6		# Shim6 Protocol [RFC5533]
wesp	141	WESP		# Wrapped Encapsulating Security Payload
rohc	142	ROHC		# Robust Header Compression
ethernet 143	Ethernet	# Ethernet encapsulation for SRv6 [RFC8986]
# The following entries have not been assigned by IANA but are used
# internally by the Linux kernel.
mptcp	262	MPTCP		# Multipath TCP connection

awk '!/^#/ && NF {print $2, $1}' /etc/protocols | sort -nr | head -n 5

262 mptcp
143 ethernet
142 rohc
141 wesp
140 shim6
