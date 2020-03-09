# Random Bits
A collection of random items

## docker and docker-compose

A few images, from scratch.

### Minimal / basic

```
cd docker-bits/basic

# build
docker build -t basic .

# run bash
docker run --rm -it basic bash
```

### Python3 image

```
cd docker-bits/python3

# build
docker build -t py3image .

# run bash
docker run --rm -it py3image bash
```

### Pytorch env (CPU)

```
cd docker-bits/pytorch-cpu

# build
docker build -t pytorch_cpu .

# run bash
docker run --rm -it pytorch_cpu bash
```
