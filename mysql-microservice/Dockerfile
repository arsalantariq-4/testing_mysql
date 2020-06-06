## Pull the mysql:5.7 image
FROM mysql:latest

## The maintainer name and email
MAINTAINER arsalan tariq <arsalan.tariq@holodeck.xyz>

# database = test and password for root = password
ENV MYSQL_DATABASE=hdprotect77 \
    MYSQL_ROOT_PASSWORD=devtest

# when container will be started, we'll have `test` database created with this schema
COPY ./test-dump.sql /docker-entrypoint-initdb.d/
