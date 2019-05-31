# https-redirect

```htcaccess
RewriteEngine on
RewriteCond %{SERVER_PORT} !^443$
RewriteRule ^(.*)$ https://%{HTTP_HOST}/$1 [QSA,R=301,L]
```
