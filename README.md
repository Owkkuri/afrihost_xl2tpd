afrihost_xl2tpd
===============

Configs for Afrihost Static IP via xl2tpd

add username & password to pap-secrets
tunnel secret is in l2tp-secrets

goto xl2tpd.conf
replace [lac username] with [lac %username provided sans the @domain.tld bit%]
replace name = user@domain.tld
