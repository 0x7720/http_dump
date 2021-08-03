# http_dump

step 1: run gencapk generate ca(ca.crt) & private key(ca.pk) \n
step 2: Add ca.crt to trusted root certificate store \n
step 3: run http_dump and waiting for local_socks data; <http_dump bind 127.0.0.1:1080>\n
step 4: write config.txt <local_socks config>\n
step 5: run local_socks\n
step 6: thk!\n
\n
local_socks:\n
 forward tun to local socks prot(config.txt); \n
\n
http_dump:\n
 dump all https request and reply; <http not supported. use Wireshark>\n
