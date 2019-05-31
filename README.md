# https-redirect

```htcaccess
RewriteEngine on
RewriteCond %{SERVER_PORT} !^443$
RewriteRule ^(.*)$ https://%{HTTP_HOST}/$1 [QSA,R=301,L]
```

```htaccess
RewriteEngine On
# редирект на другой домен
RewriteRule (.*) https://impuls-rb.ru/$1 [R=301,L]
```
