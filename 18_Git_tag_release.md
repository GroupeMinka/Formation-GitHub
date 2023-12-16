# Gérer les releases avec Git
Gérer les versions et les releases avec Git peut être une partie essentielle de la gestion de projet logiciel. 
Voici quelques bonnes pratiques pour gérer les releases avec Git (à adapter à votre fonctionnement...)

## Utiliser des branches dédiées

1. Branches de développement : Créez une branche principale pour le développement continu, souvent appelée develop ou dev.
1. Branches de fonctionnalités : Créez des branches spécifiques pour chaque nouvelle fonctionnalité ou tâche.
1. Branches de release : Créez une branche spécifique pour préparer la prochaine release à partir de la branche de développement.

## Versionnage sémantique

1. Suivez une convention de versionnement sémantique (par exemple, MAJOR.MINOR.PATCH) pour étiqueter les releases (v1.0.0, v1.1.0, etc.).
1. Utilisez des tags Git pour marquer spécifiquement les commits associés à chaque release.

## Processus de release

1. Préparation : Une fois les fonctionnalités pour une release terminées, fusionnez-les dans la branche de release depuis la branche de développement.
1. Tests : Effectuez des tests approfondis dans la branche de release pour s'assurer de la stabilité.
1. Correction de bugs : Corrigez les bugs découverts pendant les tests directement dans la branche de release.
1. Fusion finale : Fusionnez la branche de release dans master (ou main) et dans develop une fois que la release est prête à être déployée.

## Utilisation des tags
1. Créez un tag pour la version de la release une fois qu'elle est fusionnée avec succès dans la branche principale (master ou main).
1. Les tags permettent de revenir facilement à un état spécifique du code pour le déploiement ou la maintenance.

# Git tag
Les tags sont des réfs qui pointent vers des points spécifiques de l'historique Git. Les tags sont généralement utilisés pour capturer un point de l'historique utilisé pour une version.

## Création d'un tag

La création d'un tag se fait par la commande :

```Bash
git tag <tagname>
```

### Les tags annotés
Les tags annotés sont stockés comme des objets complets dans la base de données Git. Ils stockent des métadonnées supplémentaires, comme : le nom du créateur du tag, son e-mail et la date. À l'instar des commits et des messages de commit, les tags annotés possèdent un message de tag. En outre, pour des raisons de sécurité, les tags annotés peuvent être signés et vérifiés grâce à GNU Privacy Guard (GPG).
```Bash
git tag -a v1.0.1 -m "version décembre 2023"
```

### Les tags Lightweight
Les tags Lightweight sont stockés comme des objets dans la base de données Git. Ils stockent des métadonnées minimales.
```Bash
git tag v1.0.0-lw
```

**Une bonne pratique consiste à considérer les tags annotés comme publics et les tags Lightweight, comme privés.**

## Liste des tags
Pour obtenir la liste des tags d'un dépot :
```Bash
git tag

V1.0.0
    V1.0.1
    V1.0.2
    V1.0.3-rc1
    V1.0.3-rc2
```

Pour rechercher des tags
```Bash
git tag -l *rc*

    V1.0.3-rc1
    V1.0.3-rc2
```

## Pour tagger un commit
```Bash
git tag <tagname> <identifiant du commit>
```
```Bash
git tag -a <tagname> <identifiant du commit>
```

## Pour remplacer un tag existant
L'option -f (forcer) permet de mettre à jour un tag existant
```Bash
git tag -a -f <tagname> <identifiant du commit>
```

## Pour supprimer un tag
```Bash
git tag -d v1.0.2
```
