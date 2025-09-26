version de XAMP : v8.2.12
control panel : 3.3.0

<VirtualHost *:80>
    ServerName dev.local
    DocumentRoot "C:/xampp/htdocs/dev"
    <Directory "C:/xampp/htdocs/dev">
        AllowOverride All
        Require all granted
    </Directory>
    ErrorLog "logs/dev-error.log"
    CustomLog "logs/dev-access.log" combined
</VirtualHost>


C:\xampp\htdocs\dev


quand j'écris curl -i http://dev.local/, cela donne : 


C:\Users\acaliskan\Documents\bloc1\td1-architecture-web-caliskanaliisopro-dev>curl -i http://dev.local/
HTTP/1.1 200 OK
Date: Fri, 26 Sep 2025 08:54:37 GMT
Server: Apache/2.4.58 (Win64) OpenSSL/3.1.3 PHP/8.2.12
Last-Modified: Fri, 26 Sep 2025 08:45:02 GMT
ETag: "7a-63fb04d324edc"
Accept-Ranges: bytes
Content-Length: 122
Content-Type: text/html

<!DOCTYPE html>
<html>
<head><title>Dev Local</title></head>
<body><h1>Hello depuis dev.local 🚀</h1></body>
</html>