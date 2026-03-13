docker run --name graf -d grafana/Grafana
docker stats graf
docker logs graf > log.txt
docker exec graf printenv > env.txt
docker exec -it graf bash 
grafana cli admin reset-admin-password QaZoKm50

git add .
git commit -m "Добавил все файлы по дз"
git push


нужна подсказка с заданием Посмотрите список админов с помощью команды exec командой: grafana-cli admin, эта команда не работает.

