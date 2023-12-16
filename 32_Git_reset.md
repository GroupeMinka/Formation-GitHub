# Git reset
La commande git reset est utilisée pour déplacer le pointeur HEAD et éventuellement le pointeur de la branche actuelle vers un commit spécifique. Cela permet de modifier l'historique des commits et de revenir à un état antérieur du dépôt.

## Utilisation de base :

### 1. git reset avec différentes options :

--soft : Réinitialise le pointeur HEAD vers le commit spécifié tout en conservant les modifications dans l'index (staged).
--mixed (par défaut) : Réinitialise le pointeur HEAD et l'index (staging area) pour correspondre au commit spécifié tout en conservant les modifications dans le répertoire de travail.
--hard : Réinitialise complètement le pointeur HEAD, l'index et le répertoire de travail pour correspondre au commit spécifié, supprimant ainsi toutes les modifications non enregistrées.

### 2. git reset avec des références de commit :

Utilisez git reset <commit_id> pour revenir à un commit spécifique.
Vous pouvez également utiliser des références relatives comme HEAD~n pour indiquer le n-ième parent du commit actuel.

### 3. Utilisation de git reset pour déplacer des branches :

git reset --hard <commit_id> : Réinitialise la branche actuelle au commit spécifié, en déplaçant également le pointeur de branche.
git reset --soft <commit_id> : Déplace le pointeur de branche sans modifier l'index ni le répertoire de travail.

## Exercice
### Objectif :
1. Créer une série de commits.
1. Utiliser git reset pour revenir en arrière sur certains commits en conservant certaines modifications.

### Étapes :
1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide :
```bash
git init
```

2. Création d'une série de commits :
Créez un fichier (par exemple, fichier.txt) et ajoutez-y du contenu. Ensuite, effectuez plusieurs commits pour modifier progressivement ce fichier :
```bash
echo "Contenu initial" > fichier.txt
git add fichier.txt
git commit -m "Initial commit - Contenu initial"

# Apportez des modifications au fichier et effectuez plusieurs commits supplémentaires
echo "Ajout de détails" >> fichier.txt
git commit -am "Ajout de détails"

echo "Dernière modification" >> fichier.txt
git commit -am "Dernière modification"
```

3. Visualisation de l'historique des commits :
Utilisez git log pour voir l'historique des commits et notez les identifiants des commits que vous souhaitez annuler à l'aide de git reset :
```bash
git log
```

4. Utilisation de git reset pour revenir en arrière :
Utilisez git reset avec l'option appropriée (--soft, --mixed ou --hard) pour revenir en arrière sur un ou plusieurs commits. Par exemple, pour annuler le dernier commit, vous pouvez utiliser :
```bash
git reset --soft HEAD~1
```

5. Vérification et finalisation :
Après avoir utilisé git reset, vérifiez l'état du dépôt avec git status pour voir les modifications. Vous pouvez alors ré-indexer ou restaurer les fichiers selon vos besoins.
```bash
git status
```