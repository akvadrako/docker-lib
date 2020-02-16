# docker-lib

Docker image library

## Images

- build - go / gcc
- deploy - awscli / docker

## Setup

```
docker login -u akvadrako
```

## New tag

```
git commit -a
git tag v1
git push --tags

GROUP=akvadrako
NAME="${PWD##*/}"
TAG=`git describe --dirty --tags`

docker build -t $GROUP/$NAME:$TAG .
docker push $GROUP/$NAME:$TAG
```

## To trigger an automatic build

```
git push
```
