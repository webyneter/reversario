# reversario

Ansible role capable of deploying either:
* nginx stack combining [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy) with [webyneter/nginx-gen](https://github.com/webyneter/nginx-gen) and [JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion);
* [Traefik](https://docs.traefik.io/v2.0/) stack.

## Required Role Parameters

* `root_dir_path`: a path to the root directory for reversario files to reside in on a remote host e.g. `~/apps/`;
* `stack_to_launch`: a reverse proxy stack to launch on the remote host, must equal `nginx` or `traefik`;
* `letsencrypt_email`: when `stack_to_launch == traefik`, an [email](https://docs.traefik.io/v2.0/https/acme/#configuration-examples) which Let's Encrypt will send certificate expiration notices to.           

## Minimum Remote Host Requirements

* Docker (tested with 18.06)
* Docker Compose (tested with 1.22)
