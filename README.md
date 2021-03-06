# Learn Git.
> Before trying to learn how to use the CLI with git it's important for you to correctly understand how git works, you can read this article to have a good comprehension of git.
[What is version control and what is git ?](https://www.atlassian.com/git/tutorials/what-is-version-control)

## git config
```
git congif [options]
```
Cette commande permet de voir divers informations à propos de git.

## git init
```
Repo git init
```
Cette commande va tout simplement nous permettre d'installer git dans notre projet afin de pouvoir utiliser les lignes de commandes git par la suite.

## git status
```
Repo git status
```
Cette commande va nous renvoyer l'état de nos fichiers c'est-à-dire si un ou plusieurs fichiers a été crées, subis des modifications etc.. qu'il faudra si changements il y a commit afin de créer une version unique des changements.

## git log
```
Repo git log
```
Cette commande permet d'afficher l'historique des commits et de voir l'auteur, le message, la date, la clé SHA..

## git add
```
Repo git add nomDuFichier
```
Cette commande indique à git qu'il faut surveiller ce fichier si il subit des changements alors git sera qu'il a été modifé et pourra ainsi le versioner.

## git commit
```
Repo git commit [-a -m] "Entrez votre message"
```
Cette commande est l'une des plus importante elle permet à git de créer une version unique afin que le développeur puisse un jour si il le veut revenir à cette version du code, il est aussi important de définir un message avec l'option "-m". Si il faut à chaque fois de faire un commit traquer un fichier avec "git add" il est possible au moment du commit de fusioner les deux commandes afin de gagner en ajoutant les options "-a -m".

## git push
```
Repo git push origin [name of your branche]
```
Cette commande permet d'envoyer vos commits dans votre remote en l'occurence si votre code est sous GitHub(origin) dans votre branche master qui est votre branche principale la ou est déposé votre code.

## git pull
```
Repo git pull origin [name of your branche]
```
Cette commande indique à git de récupérer le code présent dans votre remote(github) sur une branche est de l'insérer dans votre repository local de ce fait vous pouvez récuperer le travail d'un autre développeur sur votre machine.

## git branch
```
Repo git branch [nom de la branche]
```
Cette commande permet soit de voir les branches crées dans notre repo ou de créer une nouvelle branche simplement en ajoutant le nom de celle-ci aprés la commande.

## git checkout
```
Repo git checkout [nom de la branche]
```
Cette commande permet de se placer dans la branche indiquée.

## git fetch
```
Repo git fetch [option]  remotename
```
La commande git fetch va récupérer toutes les données des commits effectués sur la branche courante qui n'existent pas encore dans votre version en local.

## git merge
```
Repo git merge orgin [nom de la branche]
```
Cette commande permet de mettre à jour le code de notre branche actuelle en fonction de celle indiquée.

## git blame
```
Repo git blame nomDuFichier
```
Cette commande permet de retrouver qui a modifié une ligne précise dans le fichier indiqué avec différentes informations comme l'auteur, l'heure le SHA correspondant etc..

## git show
```
Repo git show SHA
```
Cette commande permet avec un SHA correspondant de retouver le commit correspondant au SHA indiqué à combiner avec git blame qui permet de mieux visualiser le fichier et ses modifications.

## git diff
````
Repo git diff [branche-1]..[branche-2]
````
Cette commande permet de voir les différences entre la branche 1 et la branche 2 ne pas oublier les deux points entre les deux branches.

## git reset
````
Repo git reset [options]  HEAD~[nombre de commits]
````
Cette commande permet d'annuler un commit sur la branche dans laquelle on est situé

## git revert
```
Repo git revert [Sha du commit]
```
Cette commande permet d'inverser le commit qui correspond au SHA indiqué

## git stash
```
Repo git stash [options]
```
Cette commande permet de mettre les modifications en cours qui n'ont pas étés commit dans un stash CAD de coté pour que vous puissiez travailler sur autre chose

## git stash list
```
Repo git stash list
```
Cette commande permet de lister tous les stashs en cours donc tout le code qui est mit de côté en autre

## git stash pop
```
Repo git stash pop [options]
```
Cette commande permet de sortir le code du stash le plus récent donc vous récuperez votre code mit de côté

## git remote
```
Repo git remote [options]
```
Cette commande permet de lister et d'ajouter des dépots distants (copie d'un dépot sur internet)
