# grafana-prometheus-docker
default setup for installation monitoring systems into VPS

## Инсталяция на VPS
1. Установить докер ```curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh```
2. клонировать репозиторий ```git clone https://github.com/TMaksimS/grafana-prometheus-docker.git```
3. Добавить необходимые сервисы в файл **prometheus.yml**
4. Установить пароль в формате base64 в ключ _admin_ в файле **web.yml**
5. запустить весь сценарий коммандой ```docker compose -f docker-compose-grafana-prometheus.yaml up -d```
6. перейти на localhost:3000 и добавить прометея как источник данных (видео для ознакомления https://youtu.be/0hKnD4KxO5I?si=DwCyMjCV6uadN4jd). Private address: http://prometheus:9090
7. Ознакомиться с информацией из видео по постройке дашбордов.