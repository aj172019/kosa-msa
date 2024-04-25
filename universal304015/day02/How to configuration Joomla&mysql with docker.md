# How to configuration Joomla&mysql with docker
### docker-compose.yaml
```yaml
# File name should be docker-compose.yaml.
# If you name it differently, you should clarify the file name when you run the command.
version: '3.8'

services:
  joomla_db:
    image: mysql:5.7
    container_name: joomla_db
    restart: always
    environment:
      MYSQL_ROOT_PASSWORD: password
      MYSQL_DATABASE: joomla_db
    volumes:
      - /home/joomla_db:/var/lib/mysql

  joomla:
    image: joomla:4.4
    container_name: joomla
    restart: always
    ports:
      - "80:80"
    depends_on:
      - joomla_db
    environment:
      JOOMLA_DB_HOST: joomla_db
      JOOMLA_DB_USER: root
      JOOMLA_DB_PASSWORD: password
      JOOMLA_DB_NAME: joomla_db
    volumes:
      - /home/joomla_web:/var/www/html
    links:
      - joomla_db:mysql
```
```shell
touch docker-compose.yaml
vi docker-compose.yaml
# copy the above content to docker-compose.yaml
docker-compose up -d
```