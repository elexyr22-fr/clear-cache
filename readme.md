# Comment supprimé le cache Pterodatyl :

1) Liste des serveur Docker:

```
ls -lh /var/lib/pterodactyl/volumes
```

2) Pour delete un serveur docker:

```
rm -rf /var/lib/pterodactyl/volumes/<uuid_a_supprimer>
```

3) Pour clear le cache ptero + cache docker:

```
rm -rf /var/log/pterodactyl/*
docker system prune -af --volumes
```

4) Pour affiché espace disponible:

```
df -h
```

![Im 1](https://i.imgur.com/ID9mwi5.png)
