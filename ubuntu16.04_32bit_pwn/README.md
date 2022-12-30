# image

## build
```bash
docker build -t <image name>:<tag> ./
```

## pull
```bash
docker pull xeanbaek/i386-ubuntu:16.04
```

---

# container

## run
```bash
docker run -it --platform linux/386 --name i386-ubuntu xeanbaek/i386-ubuntu:16.04 /bin/bash
```

---
