# kong-gold-image-example
Example repository for building a hardened UBI8-minimal image, and then installing Kong on top, in two layers.

## Building

Simply build both images one after another:

### Base Image

```sh
docker build -t kong/base -f Dockerfile.base .
```

### Kong Image

```sh
docker build -t kong/gateway -f Dockerfile.kong .
```
