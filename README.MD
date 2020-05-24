# Docker compose repository
Proszę trzymajmy tutaj wszystkie pliki _docker-compose_,
które pomogą Nam skonfigurować lokalne środowisko

### Run locally
Dla przykładu, jeśli chcesz uruchomić _Wordpress_ & _MySQL_ uruchom poniższą komendę
```shell script
docker-compose -f mysql.yml -f wordpress.yml up
```

## MySQL

```
user     : admin
password : admin
port     : 9080
db       : wordpress
```

Jeśli chcesz przeglądać baze danych, wejdz w link `http://localhost:9080`

Domyślnie ustawia się 'wordpress' DB, możesz zmienić to przez ustawienie wartości:
```
MYSQL_DATABASE: wordpress
```
**Docker image**: https://hub.docker.com/_/mysql