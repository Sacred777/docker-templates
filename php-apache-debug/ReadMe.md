В сборке PHP 8.2, Apache, Xdebug 3.2.1

host: localhost

port: 80

Для запуска контейнера достаточно из директории docker ввести в командной строке:
`docker compose up -d`

Настройки xdebug в файле
./docker/php/xdebug.ini 

для Win 
`xdebug.client_host  = host.docker.internal`

для Linux
`xdebug.client_host  = ip_адрес_сети_докера` (часто docker0)

Можно посмотреть через
`ifconfig`

