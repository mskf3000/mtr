# mtr


(seq 1 30 | xargs -i printf '{} send-probe ip-4 35.225.133.112 ttl {} timeout 1\n') | mtr-packet

echo '35.210.165.0/24' | iprange -1 | awk '{ printf "%s send-probe ip-4 %s ttl 64 timeout 5\n", NR, $1}'
