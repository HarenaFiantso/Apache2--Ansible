# APACHE 2 x ANSIBLE
Nous savons créer des VirtualHosts de façon manuelle avec un script bash auparavant. Cette fois ci, nous allons le faire de façon automatique en utilisant un script dans un fichier d'extension .yaml sur __ANSIBLE.__

<br><br>

## __1. PREMIERE ETAPE: INSTALLATION__
#### _PREMIER CAS: INSTALLATION SIMPLE_
La première chose qu'il faut faire c'est d'installer tout d'abord __APACHE2__ dans notre système d'exploitation (Là j'utilise Manjaro):
```
sudo pacman -S apache
```
Si Apache est déjà installer dans notre système alors tant mieux. Pour le savoir, il faut exécuter la commande suivante (Pour les systèmes d'exploitation basés sur ArchLinux):

```shell
# Vérifier la version.
httpd -v

# Si Apache est installé, vous verrez la version d'Apache affichée dans la sortie du terminal. Si cela n'affiche rien du tout alors il faut exécuter la commande en dessus.
```

#### _DEUXIEME CAS: INSTALLATION AVEC ANSIBLE_
