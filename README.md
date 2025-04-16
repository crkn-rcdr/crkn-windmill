## Installation
Self-host by using Docker compose providev by windmill labs
Windmill can be deployed using 3 files: (docker-compose.yml, Caddyfile and a .env) in a single command.
Make sure Docker is started, and run:
```
curl https://raw.githubusercontent.com/windmill-labs/windmill/main/docker-compose.yml -o docker-compose.yml
curl https://raw.githubusercontent.com/windmill-labs/windmill/main/Caddyfile -o Caddyfile
curl https://raw.githubusercontent.com/windmill-labs/windmill/main/.env -o .env
docker compose up -d
```
## Config
Under the windmill_worker, create a volume to map the wip drive so that the windmill could access wip. 
e.g
 - /home/vm_account/wip:/data/wip


