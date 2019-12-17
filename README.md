### Info
github_username: Madhous

Mail: youssef.madhous@ynov.com

### Démarche de réalisation du TP
- Télécharger l'iso d'Ubuntu Server 19.10

- Télécharger VirtualBox 6.0

- Obligation d'installer la version 6.0 de VirtualBox suite à un soucis de comptabilité

- Créer une nouvelle machine virtuelle sur VirtualBox

- Mettre le disque optique d'ubuntu en premier

- Il faut faire le port Forwarding

--> Configuration -> Réseau -> Redirection de ports

- Choisir 127.0.0.1 comme IP hôte

- Choisir port d'SSH (22) comme port d'hôte

- Choisir 10.0.2.15 comme une IP invité

- Choisir 10022 comme port d'invité

- Lancer la machine virtuelle

- Installer Vagrant

```bash
sudo apt-get install vagrant
```

- Dans vagrant faire l'initialisation:
```bash
vagrant init hashicorp/bionic64
````
- Ensuite il faut ajouter les files avec la commande:
```bash
$ git add CHANGELOG.md README.md Vagrantfile
````
- Il faut configurer l'adresse mail:
```bash
$ git config --global user.email "youssef.madhous@ynov.com"
````
- Ensuite configurer le Nom:
```bash
$ git config --global user.name "madhous youssef"
````
- après, il faut sauvegarder les fichiers ajoutés avec la commande:
```bash
$ git commit -m "Add vagrantfile and docs"
````
- pour mettre à jour les références distantes avec les objets associés:
```bash
$ git push
````
- Pour installer node.js, il faut faire les commandes suivantes:
```bash
sudo apt-get update sudo apt-get install nodejs npm
````
- Installer ensuite openssh
```bash
sudo apt-get install openssh
````
- Installer nginx
```bash
sudo apt-get install nginx
````
- Lancer une invite de commandes sur Windows ou le Powershell:
Se connecter en ssh:
```bash
ssh youssef@127.0.0.1 -p 22
````