# Postgres 9.5.1 with the temporal tables extension

Start the container

    docker run --name=postgres -p 5432:5432 -d -e POSTGRES_PASSWORD=postgres skalera/postgres

Connect to the databse and enable the extension

    psql -U postgres -h localhost
    postgres=# CREATE EXTENSION temporal_tables;
