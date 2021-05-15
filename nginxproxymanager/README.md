# devops

Tools devops

## Devops Tools 1 : Nginx Proxy manager | Reverse Proxy | Certificats let's encrypt | Docker

Salut! Abonne-vous, likez si vous avez aimé et commentez si cela a fonctionné ou pas

### Ressources

> https://github.com/augustingims/devops/tree/main/nginxproxymanager

### Les références

> https://nginxproxymanager.com/

### Creation des repertoires

```bash
sudo mkdir -p ~/devops/nginx/data
sudo mkdir -p ~/devops/nginx/letsencrypt
sudo mkdir -p ~/devops/nginx/storage
```

### Configuration d'un domain en local

> sudo nano /etc/hosts

### Ajout du domain

```bash
127.0.0.1   nginxproxymanager.local
```

### Creation du network

```bash
docker network create devops_web_network
```

### Execution du service

```bash
docker-compose up -d --build
```
