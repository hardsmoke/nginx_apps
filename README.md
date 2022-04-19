# nginx_apps

```nginx
server {
	listen 80;
	root /var/www/html/app1;
}

server {
	listen 7777;
	root /var/www/html/app2;

	location /docs/ {
		alias /var/www/html/app2;
	}
}
```

![app1](https://user-images.githubusercontent.com/77721717/163954744-82bb4ae7-3c56-4fbd-8a3c-c62845c35503.png)
![app2](https://user-images.githubusercontent.com/77721717/163954756-0d35b846-37db-4e11-b33b-db529db906a4.png)
