# Derived from official mysql image (our base image)
FROM mysql:5.7
# Use mysql 5.7 as the flask-app is not set up to work with later versions

# Add a database and root password
# For hints on how to do this, consult the mysql 5.7 image documentation
ENV MYSQL_ROOT_PASSWORD=password
ENV MYSQL_DATABASE=flask-db

COPY CreateTable.sql /docker-entrypoint-initdb.d

# Add the content of the .sql file to your image
# All scripts copied to docker-entrypoint-initdb.d/ are automatically
# executed during container startup

