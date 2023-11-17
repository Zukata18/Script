# Basic Konfigurasi
system identity set name=R1
ip dhcp-client add int=eth1 en 0
ip addr add addr=21.21.21.1/29 int=eth2 
ip firewall nat add chain=srcnat action=Masquerade
ip dhcp-server setup eth2
