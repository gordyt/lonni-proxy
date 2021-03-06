# lonni-proxy

Lightweight service for serving the Zimbra NextGen app.

Required config files:

 - zimbra_server.cfg - hostname/ip address of the Zimbra SOAP server
 - ui_server.cfg - hostname/ip address of the UI server
 - server.pem - SSL certificate

## Proxy Rules

1. /beta.lonni.com -> lonni.netlify.com
2. /favicon.ico -> lonni.netlify.com/assets/favicon.ico
3. /@zimbra/<rest> -> api.zimbra.com/<rest>

## References

* [How To Implement SSL Termination With HAProxy on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-implement-ssl-termination-with-haproxy-on-ubuntu-14-04)
* [LetsEncrypt with HAProxy](https://serversforhackers.com/c/letsencrypt-with-haproxy)

