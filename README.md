afrihost_xl2tpd
===============

Configs for Afrihost Static IP via xl2tpd

add username & password to pap-secrets
tunnel secret is in l2tp-secrets

goto xl2tpd.conf
replace [lac username] with [lac %username provided sans the @domain.tld bit%]
replace name = user@domain.tld

to start / stop:

start the connection:
echo "c %name of lac%" > /var/run/xl2tpd/l2tp-control

stop the connection:
echo "d %name of lac%" > /var/run/xl2tpd/l2tp-control

You'll need your own routing-fu to send traffic over the tunnel.
