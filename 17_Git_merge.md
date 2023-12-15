# Git merge
La commande git merge est utilisée pour fusionner les modifications provenant d'une branche dans une autre. Elle est souvent utilisée pour combiner le travail effectué sur différentes branches.

## Utilisation de base

1. Fusionner une branche dans une autre :
Pour fusionner une branche spécifique (par exemple, une branche de fonctionnalité) dans la branche actuelle (généralement la branche principale), utilisez :

```bash
git merge nom_de_la_branche
```
Cela appliquera les modifications de la branche spécifiée dans la branche actuelle.

2. Résoudre les conflits :
En cas de conflits, Git vous demandera de les résoudre manuellement avant de terminer la fusion. Une fois les conflits résolus, vous pouvez finaliser la fusion en effectuant un nouveau commit.

3. Fast-forward merge :
Si la branche à fusionner est en avance linéaire par rapport à la branche actuelle, Git effectuera un "fast-forward merge". Cela signifie que Git déplacera simplement le pointeur de la branche actuelle vers le commit de la branche à fusionner.

## Exercice
### Objectif
Créer une branche, apporter des modifications, puis fusionner cette branche avec la branche principale.

### Étapes
1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide

```bash
git init
```

2. Création d'une nouvelle branche :
Créez une nouvelle branche à partir de la branche principale

```bash
git checkout -b ma_nouvelle_branche
```

3. Apporter des modifications :
Apportez des modifications à un fichier existant ou créez de nouveaux fichiers dans cette nouvelle branche.

4. Commit des modifications :
Ajoutez et committez les modifications effectuées dans cette nouvelle branche 

```bash
git add .
git commit -m "Nouvelle fonctionnalité ajoutée"
```

5. Revenir à la branche principale :
Utilisez git checkout pour revenir à la branche principale

```bash
git checkout nom_de_la_branche_principale
```

6. Fusionner la branche créée :
Fusionnez la branche que vous avez créée avec la branche principale 

```bash
git merge ma_nouvelle_branche
```

7. Vérification de la fusion :
Vérifiez que la fusion a été effectuée avec succès en examinant les modifications et en utilisant git log pour voir l'historique des commits 

```bash
git log
```
