# docker-confd

A minimalistic container for [confd](https://github.com/kelseyhightower/confd).

## Usage

```sh
docker pull aige/confd
```

For example using [Redis](http://redis.io) as backend:

```sh
docker run \
    --tty \
    --interactive \
    --rm \
    --link redis \
    aige/confd -backend=redis -node=redis:6379
```
