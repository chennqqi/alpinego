alpinego
=============

** Deplicated!!! **
Change build mode below to solve glibc linking problem

```
go build -a -installsuffix cgo
```


[![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)
[![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)
[![Docker Stars](https://img.shields.io/docker/stars/sort/alpinego.svg)](https://hub.docker.com/r/sort/alpinego/)
[![Docker Pulls](https://img.shields.io/docker/pulls/sort/alpinego.svg)](https://hub.docker.com/r/sort/alpinego/)
[![Docker Image](https://img.shields.io/badge/docker%20image-3MB-blue.svg)](https://hub.docker.com/r/sort/alpinego/)

This repository contains a **Dockerfile** of [alpinego](https://github.com/chennqqi/alpinego/) for [Docker](https://www.docker.com/)'s [trusted build](https://hub.docker.com/u/sort/alpinego/) published to the public [DockerHub](https://hub.docker.com/).

### Dependencies

-	[alpine](https://hub.docker.com/r/alpine)

### usage

1.build go app under linux  
2.write Dockerfile

`#Dockerfile`

	FROM sort/alpinego

	ARG app_name=YOU-GO-APP-BINARY  
	COPY ${app_name} /usr/bin/  
	
	ENTRYPOINT ["YOU-GO-APP-BINARY"]

### License

MIT Copyright (c) 2019-2020 **q@shellpub.com**
