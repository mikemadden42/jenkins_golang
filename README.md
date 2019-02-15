# jenkins_golang

Containerized Jenkins env to build Go projects

Use the following command to build this image.  Change the tag as needed.

```bash
docker run --rm -i hadolint/hadolint:v1.16.0 < Dockerfile
docker build -t johnnypetersringo/jenkins_golang:0.1.0 .
CI=true dive johnnypetersringo/jenkins_golang:0.1.0
docker run --rm -it johnnypetersringo/jenkins_golang:0.1.0 /bin/bash

docker login
docker push johnnypetersringo/jenkins_golang:0.1.0
docker logout
```

The Docker repository for this image can be found at:
https://hub.docker.com/r/johnnypetersringo/jenkins_golang
