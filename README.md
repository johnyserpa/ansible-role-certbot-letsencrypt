Certbot Letsencrypt (Centos 7)
=========

Minimal role to install certbot, generate letsencrypt certificates and add crons to renew certs and reload nginx.

Requirements
------------

* Centos 7
* nginx

Role Variables
--------------

Email to be used while generating certificates.

```
service_admin_email: "me@example.com"
```

Where to store letsencrypt certificates.

```
letsencrypt_ssl_dir: "/etc/letsencrypt/live/"
```

Array of domains to generate certificates.

```
ssl_domains:
  - "example.com"
  - "www.example.com"
```