# docker-php

[![github-actions](https://github.com/theohbrothers/docker-php/workflows/ci-master-pr/badge.svg)](https://github.com/theohbrothers/docker-php/actions)
[![github-release](https://img.shields.io/github/v/release/theohbrothers/docker-php?style=flat-square)](https://github.com/theohbrothers/docker-php/releases/)
[![docker-image-size](https://img.shields.io/docker/image-size/theohbrothers/docker-php/latest)](https://hub.docker.com/r/theohbrothers/docker-php)

Dockerized php with php extension(s), based on [official php images](https://hub.docker.com/_/php).

## Tags

| Tag | Dockerfile Build Context |
|:-------:|:---------:|
| `:8.2.7-fpm-alpine`, `:latest` | [View](variants/8.2.7-fpm-alpine) |
| `:8.2.7-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/8.2.7-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:8.2.7-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/8.2.7-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |
| `:8.1.23-fpm-alpine` | [View](variants/8.1.23-fpm-alpine) |
| `:8.1.23-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/8.1.23-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:8.1.23-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/8.1.23-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |
| `:8.0.30-fpm-alpine` | [View](variants/8.0.30-fpm-alpine) |
| `:8.0.30-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/8.0.30-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:8.0.30-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/8.0.30-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |
| `:7.4.33-fpm-alpine` | [View](variants/7.4.33-fpm-alpine) |
| `:7.4.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/7.4.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:7.4.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/7.4.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |
| `:7.3.33-fpm-alpine` | [View](variants/7.3.33-fpm-alpine) |
| `:7.3.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/7.3.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:7.3.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/7.3.33-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |
| `:7.2.34-fpm-alpine` | [View](variants/7.2.34-fpm-alpine) |
| `:7.2.34-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets` | [View](variants/7.2.34-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets) |
| `:7.2.34-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug` | [View](variants/7.2.34-fpm-alpine-opcache-mysqli-gd-pdo-memcached-sockets-xdebug) |

## Development

Requires Windows `powershell` or [`pwsh`](https://github.com/PowerShell/PowerShell).

```powershell
# Install Generate-DockerImageVariants module: https://github.com/theohbrothers/Generate-DockerImageVariants
Install-Module -Name Generate-DockerImageVariants -Repository PSGallery -Scope CurrentUser -Force -Verbose

# Edit ./generate templates

# Generate the variants
Generate-DockerImageVariants .
```
