# DevOps

## Ressources

>

## Les références

>

## Installation docker

> Docker

- sudo apt-get update
- sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
- curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
- sudo apt-key fingerprint 0EBFCD88
- sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
- sudo apt-get update
- sudo apt-get install docker-ce docker-ce-cli containerd.io

> Permission docker

- sudo usermod -aG docker ${USER}
- su - ${USER}
- id -nG

## Creation du stack Nginx

- Creation d'un fichier html nomme index.html qui va s'afficher lorsqu'on va acceder au nom de domain configurer en local.
- Creation d'un fichier html nomme 50x.html qui va s'afficher lorsqu'on aura une erreur 500 502 503 504.
- Creation du nginx.conf pour la configuration global de nginx
- Creation du home.conf pour acceder au nom de domain configurer en local.

## Creation du repertoire web_folder

```bash
sudo mkdir -p /opt/devops/web_folder && sudo chmod -R 777 /opt/devops/web_folder
```

## Repertoire web_folder

```
Nous devons copier index.html et 50x.html dans dossier web_folder.
```

## Configuration d'un domain en local

> sudo nano /etc/hosts

## Ajout du domain

```bash
127.0.0.1	devops.local
```

## Execution du stack

```bash
docker swarm init
docker stack deploy --compose-file tools-stack-with-nginx.yml devops
```

## Suppression du stack

```bash
docker stack rm devops
docker swarm leave --force
```
