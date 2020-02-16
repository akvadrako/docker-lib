# akvadrako/mysql-eatmydata

EatMyData wraped mysql server

Not for production use as it totally ignores fstat calls.
This container just extends mysql wrapping the server in eatmydata.

Based on https://hub.docker.com/r/interactivesolutions/eatmydata-mysql-server

## Usage

    GROUP=akvadrako
    NAME="${PWD##*/}"
    TAG=5.7.29-`git describe --dirty --tags`

    docker build -t $GROUP/$NAME:$TAG .
    docker push $GROUP/$NAME:$TAG
