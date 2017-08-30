# Docker image with java runtime


## image with jre

create image from dockerfile

```
docker build -t java .
```

Check that our image works by runing container with devault command. It should print installed java version
```
$ docker run --rm -it java
openjdk version "1.8.0_141"
OpenJDK Runtime Environment (build 1.8.0_141-8u141-b15-1~deb9u1-b15)
OpenJDK 64-Bit Server VM (build 25.141-b15, mixed mode)
```

## Running simple 'Hello' app

Build locally (with locally installed jdk) app.
```
$javac Hello.java
```

Run Hello.class on docker container
```
$ docker run -v `pwd`:/home -it -w /home java Hello
```
