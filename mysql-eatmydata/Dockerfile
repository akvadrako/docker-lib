FROM mysql:8.0.16

# Install eat my data
# RUN apt-get update && apt-get install -y eatmydata && apt-get clean
RUN apt-get update && apt-get install -y build-essential

# MySQL 8.0 requires nosync
# ADD nosync nosync.so /bin/
ADD nosync nosync
RUN cd nosync && ./configure && make && make install


# Wrap the entrypoint with eat my data
ENTRYPOINT ["nosync", "/entrypoint.sh"]

CMD ["mysqld"]
