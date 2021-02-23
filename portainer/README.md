# DevOps

## Ressources

## Les références

## Ajout du service portainer au stack

## Configuration d'un domain en local

> sudo nano /etc/hosts

## Ajout du domain

```bash
127.0.0.1	portainer.local
```

## Execution du stack

```bash
docker swarm init
docker stack deploy --compose-file tools-stack-with-portainer.yml devops
```

## Suppression du stack

```bash
docker stack rm devops
docker swarm leave --force
```
