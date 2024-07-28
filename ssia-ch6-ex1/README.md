# Before running the app create a MySql database
docker run --rm --name test-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mysql:9.0.0 && \
docker exec -it test-mysql bash
mysql -uroot -p -A
Enter password: my-secret-pw
create database spring;

# App
user: john
pwd: 12345
