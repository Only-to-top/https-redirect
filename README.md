# Редирект с http на https

```htcaccess
RewriteEngine on
RewriteCond %{SERVER_PORT} !^443$
RewriteRule ^(.*)$ https://%{HTTP_HOST}/$1 [QSA,R=301,L]
```

<h2>Редирект на другой домен</h2>

```htaccess
RewriteEngine On
RewriteRule (.*) https://new.ru/$1 [R=301,L]
```
