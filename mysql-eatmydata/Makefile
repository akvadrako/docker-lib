
NAME=akvadrako/mysql-nosync
TAG=5.7.29-`git describe --dirty --tags`

all:
	docker build -t ${NAME}:${TAG} .
	docker push ${NAME}:${TAG}
