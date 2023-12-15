# Git diff
La commande git diff est utilisée pour afficher les différences entre les changements qui ont été validés et ceux qui ne le sont pas encore dans le répertoire de travail. Elle est utile pour voir les modifications apportées à vos fichiers avant de valider ces changements.

## Utilisation de base :

### Afficher les modifications non validées :
Pour voir les modifications qui n'ont pas encore été validées, exécutez :

```bash
git diff
```
Cela affichera les différences entre les fichiers non indexés et la dernière validation (commit) réalisée.

### Afficher les différences entre des commits spécifiques :
Si vous souhaitez comparer deux commits spécifiques, utilisez la commande suivante :

```bash
git diff <commit_id_1> <commit_id_2>
```
Remplacez <commit_id_1> et <commit_id_2> par les identifiants des commits que vous souhaitez comparer.

### Afficher les différences pour un fichier spécifique :
Pour voir les modifications apportées à un fichier spécifique, utilisez :

```bash
git diff nom_du_fichier
```

### Afficher les différences avant de les valider :
Avant de valider vos modifications, vous pouvez prévisualiser les changements à valider avec :

```bash
git diff --staged
```
Cela affichera les différences entre les fichiers indexés (staged) et la dernière validation.

## Exercice

1. Créer deux fichiers texte : fichier1.txt et fichier2.txt.
1. Ajouter du contenu à ces fichiers.
1. Effectuer des modifications dans ces fichiers.
1. Utiliser git diff pour afficher les différences entre les versions non indexées et les versions indexées.

### Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide :

```bash
git init
```
### Création et édition des fichiers :
Créez fichier1.txt et fichier2.txt dans ce répertoire, ajoutez-y du contenu à l'aide d'un éditeur de texte.

### Ajout et validation des fichiers :
Utilisez les commandes suivantes pour ajouter et valider les fichiers :

```bash
git add fichier1.txt fichier2.txt
git commit -m "Ajout de fichier1.txt et fichier2.txt"
```

### Modifier les fichiers :
Modifiez le contenu de fichier1.txt et fichier2.txt en ajoutant, supprimant ou modifiant du texte.

### Utilisation de git diff :
Exécutez git diff pour voir les différences non indexées :

```bash
git diff
```

### Staging des modifications :
Ajoutez les modifications à l'index :

```bash
git add fichier1.txt fichier2.txt
```

### Nouvelle utilisation de git diff :
Affichez les différences entre les fichiers indexés et la dernière validation :

```bash
git diff --staged
```