# FlexGen-docker
FlexGen with docker


## Setup
Install Docker.

```sh
$ git clone https://github.com/hixss/FlexGen-docker
$ cd FlexGen-docker
$ docker build -t ubuntu:FlexGen .
```

## Usage
Execute following command in FlexGen-docker directory.

```sh
$ docker run -it -v /tmp:/mnt --gpus all ubuntu:FlexGen
```

In container, execute following commands.

```
root@hostname:/# cd FlexGen/flexgen/apps
root@hostname:/FlexGen# python3 completion.py --model facebook/opt-30b --percent 100 0 100 0 100 0 --compress-weight

```

# Reference
- https://agirobots.com/flexgen/
