# Run leanote in docker

1. Download latest release from https://github.com/leanote/leanote/releases
2. Unzip leanote.
3. Copy `docker-compose.yml` and `mongodb_backup` from this repo over leanote folder.
4. Update `conf/app.conf`, double check the following:
    * `db.host=db` - change to db!!!
    * `app.secret=` - change with something random, generate random string with `openssl rand -base64 32`
    * `http.addr=0.0.0.0` - be sure to set it to 0.0.0.0
5. Run a leanote instance with `docker-compose up -d`!
