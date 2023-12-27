# local-traefik
Traefik used for local env

## Allow https

Install mkcert on your system.

Launche the following command to install the local CA in the system trust store :
> mkcert -install

Generate certificates (change with your needs) :
> mkcert -cert-file certs/local-cert.pem -key-file certs/local-key.pem "*.localhost.local"

Add the configuration in file located at traefik/dynamic_conf.yaml

See traefik/dynamic_conf.yaml for example.
