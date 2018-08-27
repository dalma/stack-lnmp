# LNMP Stack

**Yuanzhen**' s Linux + Nginx + MySQL + PHP stack :)

A LNMP stack with:
 - [Nginx](https://hub.docker.com/_/nginx/) (1.14)
 - [PHP](https://hub.docker.com/_/php/) (7.2)
 - [MySQL](https://hub.docker.com/_/mysql/) (5.7)

## QuickStart

```bash
# (Build my docker images)
make build

# (Spawn up my LNMP docker stack)
make up

# (Stop and clean my stack)
make down
```

## Test

```bash

echo "Test with my web server:"
open http://localhost:8080/index.html

echo "Test with PHP environment:"
open http://localhost:8080/info.php
```
