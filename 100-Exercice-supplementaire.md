# Exercice 3 : Importer des sources locales dans un repository

# Conditions
1. J'ai des sources sur mon pc
2. J'ai développé ces sources sans utiliser GitHub.

# Etapes
1. Créer un repository sur GitHub en respectant les consignes suivantes :
* **ne pas cocher : Ajouter un readme.md**
* **ne pas sélectionner de licence**
* **ne pas sélectionner de .gitignore**

2. dans GitHub, récupérer l'adresse du repository

3. dans VS Code, ouvrir un terminal et se positionner dans le repertoire des sources

4. Affecter l'adresse du repository à votre dossier local
```Bash
git remote add origin <URL_du_repository>
```

5. Pousser les sources dans le repository
```Bash
git push origin <branch_name>
```
