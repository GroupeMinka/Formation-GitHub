# Git rm

La commande git rm est utilisée pour supprimer des fichiers du répertoire de travail et de l'index (staging area) de Git. Elle est utilisée pour indiquer à Git que vous souhaitez retirer les fichiers du suivi de version.

## Utilisation de base :

1. Supprimer un fichier suivi par Git :
Pour supprimer un fichier qui est déjà suivi par Git, utilisez :

```bash
git rm nom_du_fichier
```

Cela supprime le fichier du répertoire de travail et de l'index, et il sera donc supprimé du suivi de version lors du prochain commit.

2. Supprimer un fichier mais le conserver dans le répertoire de travail :
Si vous souhaitez simplement retirer un fichier du suivi de version sans le supprimer physiquement, utilisez l'option --cached :

```bash
git rm --cached nom_du_fichier
```

Cela retire le fichier de l'index (staging area) tout en le laissant intact dans le répertoire de travail.

3. Supprimer plusieurs fichiers en une seule commande :
Vous pouvez supprimer plusieurs fichiers en une seule commande en spécifiant les noms des fichiers à supprimer :

```bash
git rm fichier1.txt fichier2.txt
```

4. Supprimer des répertoires :
Pour supprimer un répertoire et son contenu, utilisez l'option -r (pour récursif) :

```bash
git rm -r nom_du_repertoire
```

## Exercice

### Objectif :

Créer quelques fichiers.
Utiliser git rm pour retirer ces fichiers du suivi de version.

### Étapes :

1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide :

```bash
git init
```

2. Création de fichiers :
Créez quelques fichiers dans ce répertoire :

```bash
touch fichier1.txt fichier2.txt
```

3. Ajout et commit initial :
Ajoutez ces fichiers au suivi de version et effectuez un premier commit :

```bash
git add fichier1.txt fichier2.txt
git commit -m "Ajout de fichier1.txt et fichier2.txt"
```

4. Utilisation de git rm :
Utilisez git rm pour retirer un ou plusieurs fichiers du suivi de version :

```bash
git rm fichier1.txt
```

5. Vérification avec git status :
Utilisez git status pour vérifier que le fichier a été retiré du suivi de version :

```bash
git status
```

6. Commit des modifications :
Effectuez un nouveau commit pour finaliser les changements :

```bash
git commit -m "Retrait de fichier1.txt du suivi de version"
```

