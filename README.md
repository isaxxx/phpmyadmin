# Connecting to MySQL through Docker（PHPMyAdmin）

[http://localhost:8888/](http://localhost:8888/)

## Command

### Start

```
$ docker-compose up -d
```

### Stop

```
$ docker-compose down -v
```

### Port Forwarding

```
$ ssh user@example.com -L 8889:mysql.example.com:3306 -i ./example.key -p 11111 -g
```

### Check Local IP Address (MacOS)

```
$ ifconfig
```

### Check if the Port is Used

```
$ lsof -i:8888
$ lsof -i:8889
```

### Delete Process

```
$ kill PID
```

### Confirm Server IP Address

```
$ nslookup mysql.example.com
```

### Change SSH Key to Appropriate Mode

```
$ chmod 0600 ./example.key
```

### Test SSH

```
$ ssh user@example.com -i ./example.key -p 11111
```
