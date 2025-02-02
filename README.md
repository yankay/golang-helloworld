# Standard Go Project Layout

[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5567/badge)](https://bestpractices.coreinfrastructure.org/projects/5567)

## Overview

This is a basic helloworld golang web program , just for personal use.
It would provide a GRPC,JSON,Swagger Web Interface.

## Quick Start

### Requirement

* Golang 1.7

### Compile and Run

#### Build
```
git clone https://github.com/yankay/golang-helloworld.git
cd golang-helloworld
make
```

#### Run

```
./bin/golang-helloworld
```

Access the Helloword by :
* curl http://localhost:8080/v1/ping
* Open Browser at http://localhost:8080/v1/ping
* grpcurl  -plaintext 127.0.0.1:8080 helloworld.Helloworld.Ping
* echo View API document by http://localhost:8080/swagger-ui/

#### Run for develop
```
go run cmd/main.go
```

### UnitTest

```
make test
```

### Release

```
make release # build image and release
```

### Run in Docker/Kubernetes

TODO
```
docker run *******
kubectl run ********
```
