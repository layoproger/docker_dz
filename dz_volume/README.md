# docker pull postgres:14.22-trixie
# docker run  --name dz_volume -d -v /home/vasa/data/:/data/pg postgres:14.22-trixie
# ls /home/vasa/data
# cp /home/vasa/data /home/layoshka/docker/dz_docker -r
# docker rm dz_volume
# docker run  --name dz_volume -d -v /home/layoshka/docker/dz_docker/data:/data/pg postgres:14.22-trixie

# Правда sql docker не запускался изза ошибки sql базы, нужна была регистрация.