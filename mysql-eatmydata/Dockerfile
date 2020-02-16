FROM mysql:5.7.29

# Install eat my data
# RUN apt-get update && apt-get install -y eatmydata && apt-get clean

# MySQL 8.0 requires nosync
ADD nosync nosync.so /bin/

# Wrap the entrypoint with eat my data
ENTRYPOINT ["nosync", "/entrypoint.sh"]

CMD ["mysqld"]
