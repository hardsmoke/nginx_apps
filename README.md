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
