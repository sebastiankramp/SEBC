#krb5.conf
```
[libdefaults]
default_realm = BASTI.LOCAL
dns_lookup_kdc = false
dns_lookup_realm = false
ticket_lifetime = 86400
renew_lifetime = 604800
forwardable = true
default_tgs_enctypes = aes256-cts-hmac-sha1-96
default_tkt_enctypes = aes256-cts-hmac-sha1-96
permitted_enctypes = aes256-cts-hmac-sha1-96
udp_preference_limit = 1
kdc_timeout = 3000
[realms]
BASTI.LOCAL = {
kdc = ec2-54-191-166-77.us-west-2.compute.amazonaws.com
admin_server = ec2-54-191-166-77.us-west-2.compute.amazonaws.com
ticket_lifetime = 24h
renew_lifetime = 7d
forwardable = true
}
```