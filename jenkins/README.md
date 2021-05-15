# devops

Tools devops

## Devops Tools 3 : Jenkins | Nginx proxy manager | Docker

Salut! Abonne-vous, likez si vous avez aimé et commentez si cela a fonctionné ou pas

### Ressources

> https://github.com/augustingims/devops/tree/main/jenkins

### Les références

> https://www.jenkins.io/

### Creation du repertoire jenkins_data

```bash
sudo mkdir -p ~/devops/jenkins_data
```

### Configuration d'un domain en local

> sudo nano /etc/hosts

### Ajout du domain

```bash
127.0.0.1   jenkins.local
```

### Execution du service

```bash
docker-compose up -d --build
```
