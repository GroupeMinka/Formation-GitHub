# Git add

Les commandes git add et git commit composent le workflow Git de base. Ce sont les deux commandes que chaque utilisateur de Git doit comprendre, quel que soit le modèle de collaboration de son équipe. Elles permettent d'enregistrer les versions d'un projet dans l'historique du dépôt.

## utilisation

Ajouter tous les fichiers et répertoires présents dans le workspace
```Bash
git add .
```

Ajouter tous les changements dans <fichier> pour le commit suivant.
```Bash
git add <file>
```

Ajouter tous les changements dans <répertoire> pour le commit suivant.
```Bash
git add <répertoire>
```

## Attention
Tant que le commit n'est pas fait, les fichiers et les répertoires ne sont pas inclus dans le repository local.

