# docker-parse-server

## Usage

```sh
docker run -d -p 27017:27017 --name mongo mongo
docker run -d -e APP_ID={appId} -e MASTER_KEY={masterKey} -e FILE_KEY={fileKey} --link mongo yongjhih/parse-server
```

* api: localhost:1337
* mongodb: localhost:27017

### Usage with docker-compose

```sh
wget https://github.com/yongjhih/docker-parse-server/blob/master/docker-compose.yml
docker-compose up
```

## TODO

```sh
docker run -d -e APP_ID={appId} -e MASTER_KEY={masterKey} -e API_PORT=80 -e DB_PORT=27017 yongjhih/parse-server
```

* APP_ID={myAppId}
* MASTER_KEY={mySecretMasterKey}
* FIEL_KEY={optionalFileKey}

* TODO: DB_PORT={27017}
* TODO: API_PORT={80}
* TODO: CLOUD_URL={https://github.com/yongjhih/simple-parse-cloud}
* TODO: CLOUD_PATH={/home/andrew/works/parse-server/cloud/main.js} (immutex CLOUD_URL)
* TODO: DB_URL={mongodb://localhost:27017/dev} (immutex DB_PORT)
* TODO: PARSE_SERVER_URL={https://github.com/ParsePlatform/parse-server}
* TODO: PARSE_SERVER_URL={https://github.com/ParsePlatform/parse-server/tree/2.0.0}
* TODO: PARSE_SERVER_URL={https://github.com/ParsePlatform/parse-server/tree/7f5d744}

## See Also

* https://github.com/ParsePlatform/parse-server
* http://blog.parse.com/announcements/introducing-parse-server-and-the-database-migration-tool/
* https://parse.com/docs/server/guide#migrating

## License

Apache 2.0 8tory
