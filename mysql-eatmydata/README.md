# akvadrako/mysql-eatmydata

EatMyData wraped mysql server

Not for production use as it totally ignores fstat calls.
This container just extends mysql wrapping the server in eatmydata.

Based on https://hub.docker.com/r/interactivesolutions/eatmydata-mysql-server