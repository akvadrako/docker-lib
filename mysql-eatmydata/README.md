# akvadrako/mysql-eatmydata

EatMyData wraped mysql server

Not for production use as it totally ignores fstat calls.
This container just extends mysql wrapping the server in eatmydata.

Based on https://hub.docker.com/r/interactivesolutions/eatmydata-mysql-server

## Usage

    NAME=akvadrako/mysql-nosync
    TAG=5.7.29-`git describe --dirty --tags`

    docker build -t $NAME:$TAG .
    docker push $NAME:$TAG

