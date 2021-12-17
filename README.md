# linkace-docker-sqlite
LinkAce Docker SQLite

```
git clone https://github.com/cinetube/linkace-docker-sqlite
```

```
cd linkace-docker-sqlite && chown 82:82 -R db
```

```
docker-compose up -d   
```

```
docker exec -it linkace-app-1 php artisan key:generate
```

```
docker exec -it linkace-app-1 php artisan migrate
```

```
docker exec -it linkace-app-1 php artisan registeruser
```

```
nano .env
```


change ```SETUP_COMPLETED=false``` to ```SETUP_COMPLETED=ture```


```
chmod 666 .env && chmod 777 linkace_logs/
```
