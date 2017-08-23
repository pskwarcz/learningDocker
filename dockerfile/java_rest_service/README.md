# creating simple rest service


build application
```
mvn clean install
```

create container with gs-service
```
docker build -t gs_rest_service .
```

run container with gs-service
```
docker run -it -d -p 80:8080 gs_rest_service
```

check service is working
```
curl localhost/greeting
```
