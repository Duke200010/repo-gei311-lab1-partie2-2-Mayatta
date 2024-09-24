# PARTIE 1: Collaboration sur un repository
Il faut tout d'abord :
* créer un repository dans git, 
* ajouter des collaborateurs dans settings
* mettre le repository en privé (pour éviter que tous le monde puisse faire un push dans notre repository)

La commande pour clôner un repos git distant en ligne de commande est :
```bash
 git clone https://github.com/Duke200010/6gei311-Architecture-des-logiciels
```
La commande pour ajouter tous les fichiers modifiés, supprimés et nouveau est :
```bash
 git add -a
```
La commande pour ajouter des fichiers dans le répertoire courant est :

```bash
 git add *
```
La commande pour créer une nouvelle branch dans notre repository est :

```bash
 git checkout -b [nom de la branche]
```
La commande pour changer de branche est :

```bash
 git switch [nom de la branche]
```
La commande pour faire un commit (aprés avoi fait un git add) est : 
```bash
 git commit -m [message]
```
La commande pour envoyer notre commit (nos changements) dans notre repository en ligne est :
```bash
 git push
```
La commande pour faire des update de notre branch depuis notre repos distant en local est : 
```bash
 git pull
```
La commande pour fusionner les modifications d'une branche dans la branche actuelle où on se trouve est :
```bash
 git merge [nom de la branche]
```
La commande pour voir les branches dans notre repository est : 
```bash
 git branch
```
# PARTIE 2 : SITUATIONS PROBLEMATIQUES

## SITUATION 1 : 

Pour résoudre les étapes dans la situation 1, on fait :

* Membre A doit créer un dossier localement 
* Aprés il se déplace dans le dossier créer sur le terminal a l'aide de la commande :
```bash
 cd
```
* Aprés il tape la commande pour créer un environnement git dans son dossier qui est :
```bash
 git init
```
* Pour la collaboration de B il va dans git et il crée un repository privé 
* Il va dans settings puis collaborateurs et add people et il cherche son collaborateur pour l'ajouter
* Aprés il fait : un git remote add origin avec l'url
```bash
 git remote add origin [url]
```
* Il crée une branch main : 
```bash
 git branch main
```
* On ajoute les fichiers de notre repos local avec : 
```bash
 git add -a
```
* Ensuite il fait un commit : 
```bash
 git commit -m [message]
```
* Enfin on le déploie sur notre répertoire distant avec : 
```bash
 git push -u origin main
```
## SITUATION 2 :
- On crée tout d'abord un repository dans github sous le nom de repo-gei311-lab1-partie2-2-Mayatta
- Aprés on clone le repository en faisant :
```bash
 git clone https://github.com/Duke200010/repo-gei311-lab1-partie2-2-Mayatta
```
- Aprés on crée un dossier sous le nom de dossier A en faisant :
```bash
 mkdir Dossier_A
```
- On ajoute un fichier textA.txt dans le dossier en se plaçant dans le dossier et en faisant :
```bash
 echo labo 1, gestion de version, Mayatta Ndiaye > textA.txt
```
- On ajoute les fichiers de notre repos local avec : 
```bash
 git add -a
```
- Ensuite on fait un commit : 
```bash
 git commit -m " Création du fichier text A"
```
- Pour signaler un issue on va dans la barre de recherche en haut et on appuie sur issue pour en créer un avec un titre et une description du problème contenant l'id du commit où l'erreur a été injecté.

- Pour revenir a une version ultérieure ou un de nos anciens commit on fait : 
```bash
 git reset --hard [id commit]
```
- Aprés on ajoute les fichier et on fait un commit : 
```bash
git add -a
git commit -m " Retour a la derniere verssion correcte"
```
- Aprés on le déploie dans notre serveur distant en le forçant : 
```bash
 git push -f
```
- Aprés on repars de là pour refaire les changements 