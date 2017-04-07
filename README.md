# Debug online application in alpine docker 

It's a docker image based on alpine with debug tools like tcpdump, strace, iftop, curl.

# Instructions

- Run bash

```
docker pull songrgg/alpine-debug
docker run --rm -ti songrgg/alpine-debug /bin/bash
```

- tcpdump monitors on the HTTP port

```
docker pull songrgg/alpine-debug
docker run --rm -ti songrgg/alpine-debug /bin/bash
tcpdump -A -i eth0 port 80
```

- iftop monitors current I/O

```
docker pull songrgg/alpine-debug
docker run --rm -ti songrgg/alpine-debug /bin/bash
iftop
```
