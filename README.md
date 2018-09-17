# reversario

Ansible role to dynamically add & serve anything as virtual hosts behind nginx, with automatic configuration generation and letsencrypt certificate renewal.

## Overview

Combines [webyneter/nginx-gen](https://github.com/webyneter/nginx-gen), [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy), and [JrCs/docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) into Docker Compose stack runnable on any bare-bones instance.

## Prerequisites

* Docker (tested with 18.06)
* Docker Compose (tested with 1.22)

## Required parameters

* `root_dir_path`: path to the root directory for reversario files to reside in on a remote host e.g. `~/apps/`
