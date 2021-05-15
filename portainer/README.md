# devops

Tools devops

## Devops Tools 2 : Portainer | Nginx proxy manager | Docker

Salut! Abonne-vous, likez si vous avez aimé et commentez si cela a fonctionné ou pas

### Ressources

> https://github.com/augustingims/devops/tree/main/portainer

### Les références

> https://documentation.portainer.io/

### Creation du repertoire portainer_data

```bash
sudo mkdir -p ~/devops/portainer_data
```

### Configuration d'un domain en local

> sudo nano /etc/hosts

### Ajout du domain

```bash
127.0.0.1   portainer.local
```

### Execution du service

```bash
docker-compose up -d --build
```
