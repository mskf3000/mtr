# mtr


(seq 1 30 | xargs -P1 -i printf '{} send-probe ip-4 35.225.133.112 ttl {} timeout 1\n') | mtr-packet
