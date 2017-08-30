Here we are creating image with java runtime

1. create image from dockerfile

```
docker build -t java .
```

2. we can check that our image works by runing container with devault command. It should print installed java version
```
$ docker run --rm -it java
openjdk version "1.8.0_141"
OpenJDK Runtime Environment (build 1.8.0_141-8u141-b15-1~deb9u1-b15)
OpenJDK 64-Bit Server VM (build 25.141-b15, mixed mode)
```

3. Now we will try run our own simple java app. First we will build localy (with locally installed jdk) our app.
```
$javac Hello.java
```

4. Run Hello.class on docker container
```
docker run -v `pwd`:/home -it -w /home java Hello
```
