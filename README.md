# Android Docker Build Tool Image

## Naming
### Dockerfiles
`v<Android SDK version number>_g<gradle version number>_j<java version>.Dockerfile`
### Docker image tag
`<Android SDK version number>_<gradle version number>_java<java version>.Dockerfile`

## Creation

build docker image
`docker build --file <Dockerfile> -t android:<tag> .`

check if android sdk is built correctly and optionally check if app builds correctly
`docker run -it android:latest sh`

tag docker image with username in front
`docker tag android:<tag> dweiss96/android:<tag>`

push tagged image to dockerhub
`docker push dweiss96/android:<tag>`