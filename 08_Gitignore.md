# le fichier .gitignore

## Introduction

Certains fichiers ou répertoire doivent être ignorés, donc qui ne devraient pas être commités.
Quelques exemples non exhautifs :
1. des fichiers de configuration contenant des mots de passe
2. les répertoires de compilation (en c# : \bin , \out)
3. les fichiers générés lors des tests (.log, .tmp)
4. les fichiers de configuration de l'IDE (répertoire .vscode)

## Règles d'exclusion

1. Ignorer un fichier spécifique :

```Bash
fichier.txt
```

2. Ignorer tous les fichiers avec une extension spécifique :

```bash
*.log
```

3. Ignorer tous les fichiers dans un répertoire spécifique :

```Bash
un_dossier/
```

4. Ne pas ignorer un fichier :
```Bash
# j'ignore le répertoire logs
logs/
# MAIS PAS le fichier exceptions.log
!logs/exceptions.log
```

5. Commenter vos lignes
```bash
# Ceci est un commentaire
```

Utiliser des caractères génériques pour des motifs :

? correspond à un caractère unique
* correspond à n'importe quelle séquence de caractères
** correspond à n'importe quel nombre de répertoires

6. Ignorer des fichiers par leur nom avec des caractères spéciaux échappés :

```bash
fichier\ avec\ espace.txt
```

7. Ignorer tous les fichiers d'un certain type dans un répertoire :

```bash
un_dossier/*.log
```

8. Ignorer tous les fichiers d'un certain type dans tous les répertoires :

```bash
*/*.log
```

9. Ignorer tous les fichiers dans un répertoire, mais pas le répertoire lui-même :

```bash
un_dossier/*
!un_dossier/.gitkeep
```

# Attention aux fichiers de configuration !!!
si votre projet utilise des fichiers de configuration (exemple projet.prod.env et projet.test.env), les pousser dans GitHub peut être dangereux. Les mots de passe, adresses de serveurs, ... peuvent être divulgués.

Dans vos projets, vous pouvez exclure les fichiers *.env sauf un fichier de configuration de départ
```bash
*.env
!projet.sample.env
```

le fichier projet.sample.env contient toutes les variables de configuration mais sans les valeurs.
