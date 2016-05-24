# FsInteractiveService in Docker
Dockerized [FsInteractiveService](https://github.com/ionide/FsInteractiveService) built on top of [Alpine Mono](https://hub.docker.com/r/frolvlad/alpine-mono/).

### Current version
0.1.2

### Usage
The container exposes an HTTP endpoint on port 8707.

```
$ docker run -d -p :80:8707 kerams/docker-fsinteractiveservice
3123a7b10a
$ curl -X POST http://localhost/output
{"result":"output","output":"\nF# Interactive for F# 4.0 (private)\nFreely distributed under the Apache 2.0 Open Source License\n\nFor help type #help;;\n\n> ","details":null}
```

To learn how to use FsInteractiveService head [here](http://ionide.io/FsInteractiveService/).
