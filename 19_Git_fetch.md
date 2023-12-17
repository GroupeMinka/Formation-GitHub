# Git fetch

## Qu'est-ce que git fetch ?
git fetch est une commande Git qui permet de récupérer les dernières modifications d'un dépôt distant sans fusionner ces modifications avec votre travail local. Contrairement à git pull, qui récupère les modifications et les fusionne automatiquement avec votre branche actuelle, git fetch télécharge seulement les données du dépôt distant dans votre dépôt local.

## Syntaxe de base :
La syntaxe générale de la commande git fetch est la suivante
```bash
git fetch <remote>
```
Où <remote> est le nom du dépôt distant à partir duquel vous souhaitez récupérer les modifications.

### Étapes pour utiliser git fetch
1. Lister les dépôts distants 
Pour connaître les dépôts distants associés à votre dépôt local, utilisez la commande suivante :

```bash
git remote -v
```

2. Effectuer la récupération des modifications
Pour récupérer les dernières modifications d'un dépôt distant spécifique, utilisez git fetch suivi du nom du dépôt distant. 
Par exemple, pour récupérer les modifications depuis le dépôt distant nommé "origin" :

```bash
git fetch origin
```
Cela téléchargera toutes les branches et les modifications du dépôt distant "origin" dans votre dépôt local. Cependant, ces modifications ne seront pas fusionnées automatiquement avec vos branches locales.

3. Vérifier les modifications récupérées
Vous pouvez vérifier les modifications récupérées en utilisant différentes commandes comme git log pour parcourir les commits distants ou git branch -r pour lister les branches distantes.


4. Fusionner les modifications récupérées (optionnel)
Après avoir récupéré les modifications du dépôt distant avec git fetch, vous pouvez décider de fusionner ces modifications avec vos branches locales en utilisant git merge ou git rebase.

```bash
git merge origin/<branch_name>
# ou
git rebase origin/<branch_name>
```
Remplacez <branch_name> par le nom de la branche distante que vous souhaitez fusionner avec votre branche locale.


### Astuces supplémentaires
1. Pour récupérer les modifications de toutes les branches distantes en même temps, vous pouvez utiliser git fetch --all.
1. Utilisez git fetch -p ou git fetch --prune pour supprimer les références locales qui n'existent plus sur le dépôt distant.
1. Assurez-vous de synchroniser régulièrement votre dépôt local avec les modifications du dépôt distant pour éviter les conflits potentiels.