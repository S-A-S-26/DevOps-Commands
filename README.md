# DevOps-Commands

## Docker 
1. docker ps - lists all the docker containers
2. docker status - shows the utilization status of all the containers
3. docker exec -t supabase_db_supabase pg_dump -U postgres -d postgres > /home/sujit/Databases/postgre.sql - export db from docker container -t is for terminal

## If Docker gets annoying and wont stop 
  1. sudo systemctl stop docker.socket
  2. sudo systemctl mask docker.socket

### and run when needed 
# Unmask temporarily (enables you to start it)
sudo systemctl unmask docker.socket docker.service

# Start it
sudo systemctl start docker
