https://geshan.com.np/blog/2021/12/docker-postgres/

https://www.digitalocean.com/community/tutorials/how-to-use-apache-http-server-as-reverse-proxy-using-mod_proxy-extension

Comandos docker compose:

psql:

```shell
docker compose exec db psql -U postgres -f /scripts/check.sql
```

```shell
docker compose exec db psql -U postgres -d email_sender -c 'select * from emails'
```

```shell
docker compose logs -f -t
```

Escalar o serviço

```shell
 docker compose up -d --scale worker=3
```
