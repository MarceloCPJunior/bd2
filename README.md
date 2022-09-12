# Instruções de Uso

1) acessar https://labs.play-with-docker.com/

2) no terminal rodar 
git clone https://github.com/profjosereginaldo/bd2
cd bd2
docker-compose up -d

3) clicar open port e digitar 8080

4) entrar no pgadmin4
User: pgadmin4@pgadmin.org
Password: pgadmin4

5) registrar servidor localhost
IP: 174.20.0.2
User: postgres
Password: postgres

6) criar o banco de dados academico no pgadmin4

7) no terminal rodar 
docker exec -it postgres_container /bin/bash
cd /backups
pg_restore -U postgres -d academico 20220905.backup
