
## Description
OpenVPN installation package, users can run OpenVPN service with only a small adjustment. </p>
So easy.

## System support
Rocky Linux 8

## Install
Install the RPM package, you need the `python36`、`python3-cryptography` dependency package.
```shell
# dnf install python36 python3-cryptography
# rpm -ivh OpenVPN-2.5.5-1.el8.x86_64.rpm 
Verifying...                          ################################# [100%]
Preparing...                          ################################# [100%]
Updating / installing...
   1:OpenVPN-2.5.5-1.el8              ################################# [100%]
Generating a RSA private key
.............................+++++
......................................+++++
writing new private key to 'cert/ca.key'
-----
Generating a RSA private key
.......................+++++
....................+++++
writing new private key to 'cert/server.key'
-----
Using configuration from openssl.cnf
Check that the request matches the signature
Signature ok
The Subject's Distinguished Name is as follows
countryName           :PRINTABLE:'CN'
stateOrProvinceName   :ASN.1 12:'China'
localityName          :ASN.1 12:'China'
organizationName      :ASN.1 12:'OpenVPN CA'
commonName            :ASN.1 12:'OpenVPN CA'
Certificate is to be certified until Feb 20 15:03:38 2032 GMT (3650 days)

Write out database with 1 new entries
Data Base Updated
Generating DH parameters, 2048 bit long safe prime, generator 2
This is going to take a long time
.........................................+...........................
.........................................................++*++*++*++*

Create client configure file: '/etc/openvpn/cert/cert/client.ovpn'
```
