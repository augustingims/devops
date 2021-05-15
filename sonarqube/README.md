# devops

Tools devops

## Devops Tools 4 : SonarQube | Postgres | Nginx proxy manager | Docker

Salut! Abonne-vous, likez si vous avez aimé et commentez si cela a fonctionné ou pas

### Ressources

> https://github.com/augustingims/devops/tree/main/sonarqube

### Les références

> https://www.sonarqube.org/

> https://www.sonarsource.com/

### Creation des repertoires

```bash
sudo mkdir -p ~/devops/postgres_data
sudo mkdir -p ~/devops/sonarqube_conf
sudo mkdir -p ~/devops/sonarqube_logs
sudo mkdir -p ~/devops/sonarqube_data
sudo mkdir -p ~/devops/sonarqube_extensions
```

### Configuration d'un domain en local

> sudo nano /etc/hosts

### Ajout du domain

```bash
127.0.0.1   sonarqube.local
```

### Modifier max_map_count

> sudo sysctl -w vm.max_map_count=262144

### Execution du service

```bash
docker-compose up -d --build
```
