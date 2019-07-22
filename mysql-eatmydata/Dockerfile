FROM mysql:5.5.62

# Install eat my data
RUN apt-get update && apt-get install -y eatmydata && apt-get clean

# Wrap the entrypoint with eat my data
ENTRYPOINT ["eatmydata", "/entrypoint.sh"]

CMD ["mysqld"]
