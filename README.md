### 登入 heroku

```
heroku container:login
```

### Docker 編譯

```
cd ALOHA_WEB
docker build -t alohasolution .
```

### 可加參數清快取

```
cd ALOHA_WEB
docker build -t alohasolution . --no-cache
```

### 容器推上 Heroku

```
heroku container:push -a alohasolution web
```

### 發佈

```
heroku container:release -a alohasolution web
```

### logs

```
heroku logs -a alohasolution --tail
```
