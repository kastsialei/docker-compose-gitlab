# docker-compose-gitlab
Docker-compose based on sameersbn/docker-gitlab

Check wheter postgres has enabled extension

`sudo -u postgres psql -d template1 -c "CREATE EXTENSION IF NOT EXISTS pg_trgm;"`
`sudo -u postgres -H psql -d gitlabhq_production`
`SELECT true AS enabled FROM pg_available_extensions WHERE name = 'pg_trgm' AND installed_version IS NOT NULL;`
