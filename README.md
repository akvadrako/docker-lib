# docker-lib
Docker image library

## Images

- deploy - go / awscli / docker

## Usage

```
git commit -a
git tag v1
git push --tags
git push

GROUP=akvadrako
VERSION=`git describe --dirty`

docker build -t $GROUP/deploy deploy
docker push $GROUP/deploy
```