# Git status

git status affiche l'état actuel de votre répertoire de travail et de votre zone de transit Git.
Le plus souvent utilisé sous sa forme par défaut, cela montre une bonne base d'informations sur votre écran

## options

Afficher une sortie au format court
```Bash
git status -s
```

Afficher plus de détails, y compris les modifications textuelles de tous les fichiers non validés
```Bash
git status -v
```

## Exemple
```Bash
git status
On branch main
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
   new file: sifa_sample.php
```
