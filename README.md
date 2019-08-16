# Git-Memo

## Initialiser et cloner

```git init``` : Initialise un répertoire en tant que dépôt Git <br/>
```git clone``` : Récupère un dépôt à partir d'une url (https ou ssh) <br/>

## Commiter

```git status``` : Montre les fichiers modifiés, *staged* pour le prochain commit
>On branch master
>Your branch is up to date with 'origin/master'.
>
>Changes to be committed:
>  (use "git reset HEAD <file>..." to unstage)
>
>	modified:   README.md<br/>
```git add [file]|[.]``` : *Stage* le ou les fichiers pour le prochain commit <br/>
```git reset [file]``` : *Unstage* le ou les fichiers pour le prochain commit <br/>
```git commit -m "[verbe - complément]"``` : Commite les fichiers *staged* en tant que snapshot <br/>

## Les branches, les fusions

```git branch -a``` : Liste les branches du projet. La branche suivie d'une astérisque est la branche active <br/>
>\* master
>  remotes/origin/HEAD -> origin/master
>  remotes/origin/master<br/>
```git branch [nom-branche]``` : Créé une nouvelle branche dans le commit courrant<br/>
```git checkout [nom-branche]``` : Change de branche active<br/>
```git merge [nom-branche]``` : Tente de fusionner la branche [nom-branche] avec la branche active<br/>
>**Attention** S'il y a conflit, il faut éditer les fichiers en conflits et les régler. Dans VSCode, les gestions de conflit sont faciles à gérer. Cliquer sur *incoming changes* pour garder les changements du côté serveur par exemple.<br/>
