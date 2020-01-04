# Dicas

- Linha de comando do PostgreSQL
  docker-compose run --rm db psql

- Backup de um banco via ip
  docker-compose run --rm db pg_dump --host XXX.XXX.XXX.XXX --port 5432 --username "seu_usuario" --dbname "seu_db_production" --format tar --file "./YYYY.MM.DD"

- Restore db
  docker-compose run --rm db pg_restore --host db --port 5432 --username "seu_usuario" --dbname "seu_db_development" --verbose "/root/YYYY.MM.DD"
