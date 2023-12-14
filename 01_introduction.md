# Formation Github - Visual Studio Code

## Introduction

### 1. Contôle de version

Le contrôle de version, également connu sous le nom de contrôle de source, est une pratique essentielle dans le développement logiciel, visant à suivre et gérer les modifications apportées au code d'un programme. Les systèmes de contrôle de version sont des outils logiciels permettant aux équipes de développement de gérer efficacement ces changements au fil du temps. Ces systèmes sont cruciaux pour accélérer les environnements de développement, aidant les équipes DevOps à travailler de manière plus agile et efficiente. Ils maintiennent une base de données spéciale qui trace chaque modification du code, offrant ainsi la possibilité aux développeurs de revenir à des versions antérieures en cas d'erreur, minimisant ainsi les perturbations pour l'ensemble de l'équipe.

### 2. Pourquoi utiliser un outil de contrôle de version

1. Historique complet : Les VCS conservent un historique détaillé des modifications effectuées sur chaque fichier, permettant aux équipes de remonter le temps pour analyser les raisons des erreurs et des bugs, même dans d'anciennes versions du logiciel.

2. Branchement et fusion (merges) : Ils offrent la possibilité de créer des branches pour travailler sur des flux de changements distincts, facilitant ainsi la gestion de multiples tâches parallèles tout en permettant la fusion des modifications pour éviter les conflits.

3. Traçabilité : Les VCS offrent une traçabilité précise de chaque modification, permettant de lier les changements à d'autres outils de gestion de projet et de suivi des bugs comme Jira. Cette traçabilité facilite l'analyse des causes profondes des problèmes, permettant aux développeurs de comprendre, d'annoter et de modifier le code de manière cohérente et anticipée.

### 3. un peu d'histoire

| Année | Outil             | Description                                           |
|-------|-------------------|-------------------------------------------------------|
| 1972  | RCS (Revision Control System) | Système de contrôle de versions initial, permettant le suivi des modifications dans les fichiers. |
| 1982  | CVS (Concurrent Versions System) | Évolution du RCS, permettant le travail simultané sur des fichiers et la gestion de versions concurrentes. |
| 2000  | SVN (Subversion)  | Successeur de CVS, apportant des améliorations en termes de fonctionnalités et de gestion de versions. |
| 2005  | Git               | Système de contrôle de version distribué, rapide et flexible, développé par Linus Torvalds. |
| 2008  | GitHub            | Plateforme d'hébergement pour les projets Git, offrant des fonctionnalités de collaboration et de gestion de code source. |
| 2008  | Bitbucket         | Plateforme de gestion de code source utilisant Mercurial et Git, avec des fonctionnalités de collaboration et d'intégration. |
| 2011  | GitLab            | Plateforme complète de gestion du cycle de vie des applications, offrant des fonctionnalités de DevOps et de gestion de code source. |


### 4. ligne de commande vs interface

Bien que les interfaces graphiques comme celle proposée par VSCode facilitent beaucoup l'utilisation de Git et GitHub, il est bénéfique de connaître les commandes de base de Git en ligne de commande. La ligne de commande permet d'accéder à des fonctionnalités plus avancées de Git et de résoudre des problèmes spécifiques qui pourraient ne pas être pris en charge par les interfaces graphiques.

### 5. Visual Studio Code (vsc)
Visual Studio Code (VS Code) est un éditeur de code très populaire, et bien qu'il ne soit pas un environnement de développement intégré (IDE) complet dans le sens traditionnel, il présente plusieurs avantages par rapport à d'autres IDE :

1. Léger et rapide : VS Code est léger par rapport à de nombreux IDE, ce qui le rend rapide à démarrer et à utiliser. Il consomme moins de ressources système tout en offrant des performances rapides.

2. Personnalisable : Il offre une grande flexibilité pour personnaliser l'interface utilisateur, les thèmes, les raccourcis clavier et les fonctionnalités à l'aide d'une vaste gamme d'extensions disponibles dans le marché des extensions de VS Code.

3. Polyvalent : VS Code prend en charge un large éventail de langages de programmation, offrant des outils et des extensions spécifiques pour de nombreuses technologies, ce qui en fait un choix polyvalent pour les développeurs travaillant sur divers projets.

4. Intégration Git : L'intégration native avec Git permet de gérer facilement les versions du code source directement depuis l'éditeur.

5. Débogage efficace : Il offre des fonctionnalités de débogage robustes pour plusieurs langages, permettant aux développeurs de localiser et de résoudre les erreurs plus efficacement.

6. Support multiplateforme : Disponible sur Windows, macOS et Linux, VS Code offre une expérience cohérente sur différentes plateformes, ce qui le rend accessible à un plus large éventail de développeurs.

7. Communauté active : Avec une communauté très active, il existe une abondance de ressources, de tutoriels et de forums en ligne pour aider les utilisateurs à résoudre les problèmes et à améliorer leurs compétences.

8. Mises à jour fréquentes : Microsoft et la communauté open source publient régulièrement des mises à jour et des améliorations, ajoutant de nouvelles fonctionnalités et améliorant la stabilité de l'outil.

9. Intégration d'outils externes : VS Code peut être étendu avec des outils externes, ce qui permet d'intégrer des fonctionnalités supplémentaires sans alourdir l'éditeur de base.