# docker-lib

Docker image library

## Images

- build - go / gcc
- deploy - awscli / docker

## Setup

```
docker login
```

## New tag

```
git commit -a
git tag v1
git push --tags

GROUP=akvadrako
TAG=`git describe --dirty --tags`

docker build -t $GROUP/deploy:$TAG deploy
docker push $GROUP/deploy:$TAG
```

## To trigger an automatic build

```
git push
```