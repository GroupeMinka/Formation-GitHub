# Git revert
La commande git revert est utilisée pour annuler des modifications spécifiques en créant un nouveau commit qui inverse les changements effectués par un ou plusieurs commits existants.

## Utilisation de base :
### 1. Revenir en arrière sur un commit spécifique :
Pour annuler les changements apportés par un commit spécifique, utilisez :

```bash
git revert <commit_id>
```
Remplacez <commit_id> par l'identifiant du commit que vous souhaitez annuler. Cela créera un nouveau commit qui annulera les changements du commit spécifié.

### 2. Revenir en arrière sur plusieurs commits :
Si vous souhaitez annuler les changements de plusieurs commits, vous pouvez spécifier une plage de commits en utilisant la syntaxe suivante :

```bash
git revert <commit_id_1>..<commit_id_2>
```
Cela annulera les modifications incluses dans la plage de commits spécifiée.

### 3. Résoudre les conflits :
Il est possible que des conflits surviennent lors de l'application du revert. Dans ce cas, Git vous demandera de résoudre ces conflits avant de finaliser le commit revert.


## Exercice

### Objectif :
Créer un nouveau fichier et effectuer plusieurs commits avec des modifications progressives.
Utiliser git revert pour annuler sélectivement certains de ces commits.

### Étapes :
1. Initialisation du dépôt Git :
Commencez par initialiser un nouveau dépôt Git dans un dossier vide :

```bash
git init
```

2. Création d'un fichier et premiers commits :
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
Utilisez git log pour voir l'historique des commits et notez les identifiants des commits que vous souhaitez annuler à l'aide de git revert :

```bash
git log
```

4. Revert d'un ou plusieurs commits :
Utilisez git revert pour annuler sélectivement un ou plusieurs commits en utilisant les identifiants des commits que vous avez notés :

```bash
git revert <commit_id>
```

5. Résolution de conflits (si nécessaire) :
Si des conflits surviennent lors de l'application du revert, résolvez-les en modifiant les fichiers concernés et en utilisant les commandes Git pour marquer les conflits comme résolus (git add, git commit).

6. Vérification et finalisation :
Après avoir annulé les commits, vérifiez le statut du dépôt avec git status. Une fois satisfaits des modifications, créez un nouveau commit pour finaliser le revert.