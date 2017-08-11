# learningDocker

## usuig Docker with boot2docker behind corporate proxy

```
sudo vi /var/lib/boot2docker/profile
```

add:

```
export "HTTP_PROXY=http://proxy:3128"
export "HTTPS_PROXY=http://proxy:3128"
export "NO_PROXY=192.168.23.4"
```
