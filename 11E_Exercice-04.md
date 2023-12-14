# Exercice 4 : Effectuer des modifications et les réintégrer dans les sources du projet

## Intro
Nous allons sur le projet ExerciceSifa-1 :

1. Modifier le fichier style.css
1. Effectuer un commit 
1. Visualiser les modifications du commit
1. Modifier le fichier index.html pour ajouter un sous-titre 4 de couleur bleue
1. Ajouter un fichier test.html
1. Effectuer un commit 
1. Visualiser les modifications du commit
1. Constater les changements dans github

## Pour vous aider
Contenu à ajouter au fichier style.css : cette partie de code permet d'affecter la couleur verte au sous-titre.
```css
h2 {color:green}
```

Contenu à ajouter dans le fichier index.html :
```html
<h2 style="color:blue">Sous-titre 5</h2>
```

contenu du fichier test.html
```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <!-- Chargement de la feuille de style -->
        <link rel="stylesheet" href="./style.css">
        <!-- Titre de la page -->
        <title>Exercice 4</title>
    </head>
    <body>
        <h1>Exercice 4</h1>
        <h2>Et non, ce n'est pas un Hello World !</h2>
    </body>
</html>
```

