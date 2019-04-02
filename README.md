alpinego
=============

[![Circle CI](https://circleci.com/gh/chennqqi/alpinego.png?style=shield)](https://circleci.com/gh/malice-plugins/clamav)
[![License](http://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)
[![Docker Stars](https://img.shields.io/docker/stars/malice/clamav.svg)](https://hub.docker.com/r/sort/alpinego/)
[![Docker Pulls](https://img.shields.io/docker/pulls/malice/clamav.svg)](https://hub.docker.com/r/sort/alpinego/)
[![Docker Image](https://img.shields.io/badge/docker%20image-188MB-blue.svg)](https://hub.docker.com/r/sort/alpinego/)

This repository contains a **Dockerfile** of [alpinego](https://github.com/chennqqi/alpinego/) for [Docker](https://www.docker.io/)'s [trusted build](https://index.docker.io/u/sort/alpinego/) published to the public [DockerHub](https://index.docker.io/).

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
