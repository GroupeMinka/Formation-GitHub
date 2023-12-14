# Exercice 2 : Cloner manuellement un repository

## Introduction
Je veux cloner un repository dans le répertoire <User>\Projects\ExerciceSifa-1-2

La commande git clone permet de récuperer en local un repository.

```bash
 git clone <url_du_repository> [<repertoire>]
```

si l'information <repertoire> n'est pas fournie, le repository sera copié dans un repertoire portant le nom du repository.


## 1. Ouvrir un terminal dans VS Code

Menu déroulant "Affichage" -> commande "Terminal"

## 2. Cloner un repository

git clone <url_du_repository> <repertoire>

```bash
PS C:\Users\Laurent\Projects> git clone https://github.com/lgrdev/ExerciceSifa-1.git ExerciceSifa-1-2
Cloning into 'ExerciceSifa-1'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
PS C:\Users\Laurent\Projects> cd ExerciceSifa-1-2
PS C:\Users\Laurent\Projects\ExerciceSifa-1-2> dir


    Répertoire : C:\Users\Laurent\Projects\ExerciceSifa-1-2


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        03/12/2023     10:17             48 README.md


PS C:\Users\Laurent\Projects\ExerciceSifa-1-2> 
```
