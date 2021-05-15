# devops

Tools devops

## Devops Tools 5 : Adminer | Mysql | Nginx proxy manager | Docker

Salut! Abonne-vous, likez si vous avez aimé et commentez si cela a fonctionné ou pas

### Ressources

> https://github.com/augustingims/devops/tree/main/adminer

### Les références

> https://www.adminer.org/

### Creation du repertoire mysql_data

```bash
sudo mkdir -p ~/devops/mysql_data
```

### Configuration d'un domain en local

> sudo nano /etc/hosts

### Ajout du domain

```bash
127.0.0.1   adminer.local
```

### Execution du service

```bash
docker-compose up -d --build
```
