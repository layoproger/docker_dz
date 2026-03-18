docker run --name my_redis -p 6379:6379  -d redis
docker ps
docker logs my_redis | grep "Ready to accept connections"
docker logs my_redis > redis_log.txt
docker exec my_redis env > redis_env.txt
docker exec -it my_redis bash
redis-cli PING
redis-cli SET mykey "Hello Docker"
redis-cli GET mykey
exit
docker stats my_redis
CONTAINER ID   NAME       CPU %     MEM USAGE / LIMIT    MEM %     NET I/O         BLOCK I/O     PIDS
28cdd014a552   my_redis   0.24%     30.7MiB / 1.608GiB   1.86%     1.16kB / 126B   54.2MB / 0B   6
1