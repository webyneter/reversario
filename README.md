# ansible-role-reversario

Dynamically add & serve anything as virtual hosts behind nginx, with automatic configuration generation and letsencrypt certificate renewal.

## Overview

Combines [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy), [jwilder/docker-gen](https://index.docker.io/u/jwilder/docker-gen/) and [JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) into Docker Compose stack runnable on your bare-bones deployment instance.

## Prerequisites

* Docker (tested with 18.06)
* Docker Compose (tested with 1.22)
