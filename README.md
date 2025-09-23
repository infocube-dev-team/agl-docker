# AGL dev environment
AGL local development environment


## Project structure
Setup a folder structure like this:
```
agl
├── agl-config-page-composition
├── agl-config-server
├── agl-core
├── agl-custom-middleware
├── agl-docker (this folder)
└── agl-gulp
```


## Elasticsearch
Import a valid dump into elasticsearch container


## Git setup
If you're not able to clone projects using git+ssh, run this command:
```
git config --global url.https://rit.accenture.com/avs-bitbucket/scm/.insteadOf ssh://git@rit.accenture.com:8080/
```
this will re-route git+ssh to git+https


## Clone
Clone needed AGL project 
```
git clone https://rit.accenture.com/avs-bitbucket/scm/agl/004-agl-config-server.git agl-config-server
git clone https://rit.accenture.com/avs-bitbucket/scm/agl/004-agl-core.git agl-core
git clone https://rit.accenture.com/avs-bitbucket/scm/agl/004-agl-page-composition-middleware.git agl-custom-middleware
git clone https://rit.accenture.com/avs-bitbucket/scm/avs-m3/004-agl-gulp.git agl-gulp
```


## Install
Install dependencies in all the folders with
```
npm install
```


## Start
```
docker compose up -d
```


## Service endpoints example
Services should then be available:

agl-config-server: 
- [/app/config](http://localhost:3004/app/config)

agl-core:
- [/TRAY/SEARCH/VOD](http://localhost:3000/AGL/1.5/A/ENG/CHROME_HTML5/ALL/TRAY/SEARCH/VOD)
