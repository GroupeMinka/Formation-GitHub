# Git clean

La commande git clean est utilisée pour supprimer les fichiers non suivis (non indexés) du répertoire de travail. Elle est utile pour nettoyer le répertoire des fichiers non désirés qui ne sont pas suivis par Git.

## Utilisation de base :

### 1. Afficher les fichiers non suivis :
Avant de supprimer les fichiers, vous pouvez afficher les fichiers non suivis pour comprendre ce qui sera effacé. Utilisez la commande :

```bash
git clean -n
```

Cela affichera une liste des fichiers non suivis qui seront supprimés si vous exécutez git clean sans -n.

### 2. Supprimer les fichiers non suivis :
Pour supprimer réellement les fichiers non suivis, exécutez :

```bash
git clean -f
```

Assurez-vous d'être prudent en utilisant -f car cela supprime définitivement les fichiers. Cette commande supprimera les fichiers non suivis répertoriés par git clean -n.

### 3. Supprimer récursivement les répertoires non suivis :
Pour supprimer également les répertoires non suivis, utilisez l'option -d avec -f :

```bash
git clean -fd
```
## Exercice
1. Créer quelques fichiers et répertoires non suivis.
2. Utiliser git clean pour supprimer ces fichiers et répertoires non suivis.

### Étapes :
1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide :

```bash
git init
```

2. Création de fichiers et répertoires non suivis :
Créez quelques fichiers et répertoires non suivis dans ce répertoire. Vous pouvez le faire en utilisant la commande touch pour créer des fichiers vides et mkdir pour créer des répertoires.

```bash
touch fichier1.txt fichier2.txt
mkdir dossier1 dossier2
```

3. Vérification des fichiers non suivis :
Utilisez git status pour vérifier quels fichiers et répertoires sont non suivis :

```bash
git status
```

4. Prévisualisation des fichiers à supprimer :
Utilisez git clean -n pour prévisualiser les fichiers et répertoires non suivis qui seront supprimés :

```bash
git clean -n
```

5. Suppression des fichiers non suivis :
Pour supprimer les fichiers non suivis répertoriés, exécutez :

```bash
git clean -f
```

6. Vérification finale :
Vérifiez à nouveau l'état du répertoire après avoir utilisé git clean :

```bash
git status
```
