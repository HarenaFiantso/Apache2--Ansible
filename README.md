# APACHE 2 x ANSIBLE
Nous savons créer des VirtualHosts de façon manuelle avec un script bash auparavant. Cette fois ci, nous allons le faire de façon automatique en utilisant un script dans un fichier d'extension .yaml sur __ANSIBLE.__

<br><br>

## __1. PREMIERE ETAPE: INSTALLATION__
#### _INSTALLATION D'APACHE:_
La première chose qu'il faut faire c'est d'installer tout d'abord __APACHE2__ dans notre système d'exploitation (Là j'utilise Manjaro):
```shell
sudo pacman -Sy
sudo pacman -S apache

# ou

pamac install apache

# ou

yay -S apache
```
Si Apache est déjà installer dans notre système alors tant mieux. Pour le savoir, il faut exécuter la commande suivante (Pour les systèmes d'exploitation basés sur ArchLinux):

```shell
# Vérifier la version.
httpd -v

# Si Apache est installé, vous verrez la version d'Apache affichée dans la sortie du terminal. Si cela n'affiche rien du tout alors il faut exécuter la commande en dessus.
```

#### _INSTALLATION D'ANSIBLE:_
Pour installer __ANSIBLE__ sur Manjaro, vous pouvez suivre les étapes ci-dessous :
```shell
sudo pacman -S ansible
```
Une fois l'installation terminée, on doit avoir __ANSIBLE__ installé sur votre système Manjaro.

<br>

Vous pouvez vérifier si __ANSIBLE__ est installé en exécutant la commande suivante pour afficher la version d'__ANSIBLE__ :
```shell
ansible --version

# ou

pacman -Q | grep ansible

```

Cela devrait afficher des informations sur la version d'Ansible installée sur votre système.

Maintenant, vous pouvez utiliser Ansible pour automatiser des tâches de configuration et de déploiement sur vos hôtes cibles.