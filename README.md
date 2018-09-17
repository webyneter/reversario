# reversario

Ansible role deploying [webyneter/nginx-gen](https://github.com/webyneter/nginx-gen), [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy), and [JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) Docker Compose stack allowing for dynamic addition and removal of your apps as virtual hosts behind nginx, with automatic configuration generation and letsencrypt certificate issuance.

## Remote host prerequisites

* Docker (tested with 18.06)
* Docker Compose (tested with 1.22)

## Required role parameters

* `root_dir_path`: path to the root directory for reversario files to reside in on a remote host e.g. `~/apps/`
