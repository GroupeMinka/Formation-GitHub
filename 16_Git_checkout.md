# Git checkout
La commande git checkout est utilisée dans Git pour naviguer entre les branches, les tags, ou pour modifier les fichiers dans le répertoire de travail. Elle peut être utilisée pour effectuer plusieurs tâches différentes.

## Utilisation de base

### 1. Changer de branche :
Pour passer à une branche spécifique, utilisez :

```Bash
git checkout nom_de_la_branche
```
Cela vous fait basculer vers la branche spécifiée.

### 2. Créer et basculer vers une nouvelle branche :
Pour créer une nouvelle branche et basculer vers celle-ci en une seule commande, utilisez -b :

```Bash
git checkout -b nouvelle_branche
```
Cela crée une nouvelle branche à partir de la branche actuelle et vous fait basculer vers cette nouvelle branche.

### 3. Basculer vers un commit spécifique :
Vous pouvez également basculer vers un commit spécifique en utilisant son identifiant :

```Bash
git checkout identifiant_commit
```
Cela vous positionne sur ce commit en mode détaché (vous n'êtes pas sur une branche).

### 4. Annuler les modifications non enregistrées :
Utilisez git checkout pour annuler les modifications non enregistrées d'un fichier :

```Bash
git checkout nom_du_fichier
```
Cela restaure la version du fichier telle qu'elle est dans l'index (staging area) ou dans le dernier commit.

## Exercice
### Objectif :
Créer une nouvelle branche, apporter des modifications et ensuite revenir à la branche principale.

### Étapes :
1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide 
```Bash
git init
```
2. Création d'une nouvelle branche :
Créez une nouvelle branche à partir de la branche principale 
```Bash
git checkout -b ma_nouvelle_branche
```

3. Apporter des modifications :
Apportez des modifications à un fichier existant ou créez de nouveaux fichiers.

4. Vérification des modifications :
Utilisez git status pour voir les modifications apportées dans la nouvelle branche 
```Bash
git status
```

5. Revenir à la branche principale :
Utilisez git checkout pour revenir à la branche principale
```Bash
git checkout nom_de_la_branche_principale
```

6. Vérification du changement de branche :
Vérifiez que vous êtes bien revenu à la branche principale en utilisant git branch pour afficher toutes les branches
```Bash
git branch
```

