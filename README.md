## Installation
Windmill container can be deployed using 3 files: docker-compose.yml, Caddyfile and a .env
1. Create a .env file based on .env.sample, and set the POSTGRES_PASSWORD and POSTGRES_DB values. These values are referenced in docker-compose.yml.
2. Under the windmill_worker on the docker-compose.yml, create a volume to map the wip drive so that the windmill could access wip. 
e.g.,
 - /home/vm_account/wip:/data/wip
 - /home/vm_account/ocr:/data/ocr
3. To build a windmill_container by:
```
docker compose up -d 
```
## Wmill CLI installation
To install the wmill CLI:
```
npm install -g windmill-cli
```
Notes: Node need to be installed before install wmill and the Node version must greater than v20.
Reference : See https://www.windmill.dev/docs/advanced/cli/installation
## Git sync
All scripts, flows and apps located in the workspace will be pushed to the Git repository. So git need to be installed for using git sync
Reference : See https://www.windmill.dev/docs/advanced/git_sync
## Windmill Docs
See the https://github.com/windmill-labs/windmill and https://www.windmill.dev/docs/advanced/self_host


