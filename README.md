# xoops2.59
這包預設跑起來可以上傳的大小是100MB
```
docker run --name mysql -e MYSQL_ROOT_PASSWORD=你的密碼 -p 3306:3306 -d mysql

docker run --name phpmyadmin --link mysql:db -p 8088:80 -d phpmyadmin/phpmyadmin

docker run --name xoops --link mysql:db -p 80:80 -d jahaulin/xoops
```
