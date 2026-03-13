# дз по базе docker
docker run --name graf -d grafana/Grafana
docker stats graf
docker logs graf > log.txt
docker exec graf printenv
docker exec -it graf bash 
grafana cli admin reset-admin-password QaZoKm50

