# Git Stash

git stash est une commande Git permettant de sauvegarder temporairement des modifications locales non validées (non commité) dans un espace de travail propre. Cela vous permet de basculer entre différentes tâches ou branches sans avoir à valider ou à commiter vos modifications en cours.

Le stashing est pratique si vous avez besoin de changer rapidement de contexte et de travailler sur autre chose, mais que vous êtes en plein dans un changement de code et que n'êtes pas tout à fait prêt à commiter.

## Étapes pour utiliser git stash :

### Étape 1 : Vérification de l'état actuel du dépôt
Avant de commencer, vérifiez l'état de vos modifications en utilisant la commande :
```bash
git status
```

### Étape 2 : Stasher les modifications
Si vous avez des modifications que vous ne souhaitez pas valider pour le moment, utilisez git stash :

```bash
git stash save "Description de votre stash (optionnel)"
```
Cela enregistrera vos modifications dans un stash avec une description optionnelle pour une référence future.

### Étape 3 : Vérification des stashes
Pour voir la liste des stashes enregistrés, utilisez la commande :

```bash
git stash list
```
Cela affichera les différents stashes avec des identifiants uniques (stash@{n}) et des descriptions si fournies.

### Étape 4 : Appliquer un stash
Si vous souhaitez appliquer les modifications d'un stash spécifique, utilisez la commande git stash apply suivi de l'identifiant du stash (par exemple, stash@{1}) :

```bash
git stash apply "stash@{1}"
```
### Étape 5 : Supprimer un stash
Après avoir appliqué les modifications et les avoir réintégrées dans votre travail, vous pouvez supprimer le stash avec la commande :

```bash
git stash drop "stash@{1}"
```
Cela supprimera le stash spécifique.

### 'git stash apply' vs 'git stash pop' 
La principale différence réside dans le fait que le « git stash pop » applique vos modifications à votre répertoire de travail actuel mais il supprime également le cache de la pile de cache.

### voir le contenu d'un cache
```bash
git stash show "stash@{1}"
git stash show -p "stash@{1}"
```

## Exercice :

1. Créez un nouveau fichier example.txt.
2. Ajoutez-y quelques lignes de texte.
3. Effectuez un git status pour voir les modifications non validées.
4. Utilisez git stash pour mettre de côté ces modifications.
5. Vérifiez la liste des stashes avec git stash list.
6. Supprimez les modifications de votre espace de travail avec git stash drop stash@{0} (Assurez-vous de remplacer {0} par le bon identifiant du stash si nécessaire).
7. Vérifiez à nouveau l'état de votre répertoire avec git status. Vous devriez voir un espace de travail propre sans modifications.
8. Appliquez à nouveau le stash que vous avez précédemment enregistré avec git stash apply.
9. Vérifiez que les modifications sont bien réappliquées à votre espace de travail.
10. Supprimez ce stash avec git stash drop stash@{0}.