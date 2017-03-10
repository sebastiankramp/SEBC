logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log  


[libdefaults]
default_realm = SEBASTIANKRAMP.ES
dns_lookup_kdc = false
dns_lookup_realm = false
ticket_lifetime = 86400
renew_lifetime = 604800
forwardable = true
default_tgs_enctypes = aes256-cts
default_tkt_enctypes = aes256-cts
permitted_enctypes = aes256-cts
udp_preference_limit = 1
kdc_timeout = 3000
default_principal_flags = +renewable

[realms]
SEBASTIANKRAMP.ES = {
kdc = ec2-54-191-166-77.us-west-2.compute.amazonaws.com
admin_server = ec2-54-191-166-77.us-west-2.compute.amazonaws.com
}
