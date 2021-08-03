# http_dump

step 1: run gencapk generate ca(ca.crt) & private key(ca.pk)
step 2: Add ca.crt to trusted root certificate store
step 3: run http_dump and waiting for local_socks data; <http_dump bind 127.0.0.1:1080>
step 4: write config.txt <local_socks config>
step 5: run local_socks
step 6: thk!

local_socks:
 forward tun to local socks prot(config.txt); 

http_dump:
 dump all https request and reply; <http not supported. use Wireshark>
