# Les conflits et comment les résoudre
Lorsque l’on travaille sur un projet en équipe, il est courant de rencontrer des conflits d’édition ou fusion de code. Et quelque part, cette situation est normale.

## Conflit ?

Définition par [Atlassian](https://www.atlassian.com/fr/git/tutorials/using-branches/merge-conflicts){:target="_blank"}  : 
Les conflits surviennent généralement lorsque deux personnes ont modifié les mêmes lignes dans un fichier, ou si un développeur a supprimé un fichier alors qu’un autre développeur le modifiait. 
Dans ces cas, Git ne peut pas déterminer automatiquement la version correcte. Les conflits n’affectent que le développeur qui effectue le merge, les autres membres de l’équipe ne sont pas conscients du conflit. 
Git marquera le fichier comme étant en conflit et arrêtera le processus de merge. Il incombe alors aux développeurs de résoudre le conflit.

![conflit_01](./images/github/conflit_01.png)

## Les cas de conflit
1. **Modification concurrente** : quand plusieurs développeurs modifient la même ligne de code d’un même fichier et tentent de fusionner le changement sur une même branche ; quand les changements contenus d'un commit portent sur le même fichier ou ligne(s) de code.
2. **Suppression de code / fichier** : quand un développeur supprime un fichier (ou une ligne), qu’un autre développeur a édité ce fichier ou cette ligne, et que chacun des deux cherchent à fusionner sa modification sur une même branche.
3. **Déplacement ou renommage de fichier** : quand un développeur renomme ou déplace un fichier, pendant que dans le même temps, un autre développeur y a apporté des modifications
4. **Fusion de branches** : lorsqu’un développeur souhaite intégrer une branche sur une autre, toutes deux ayant subies des modifications aux mêmes endroits, ex : au moment de fusionner une pull request, opération consistant à réintégrer la branche Git correspondante sur la branche principale du repository.
4. **Rebasage de branche** : lorsque l’on effectue une opération de rebasage (“action consistant à décaler une série de commits”) sur une branche

## Comment éviter les conflits ?
1. **Utiliser les branches** : En utilisant des branches, on évite les conflits durant le développement des fonctionnalités => on se concentre sur le dev
2. **Synchroniser régulièrement** : il faut rebaser très souvent et très régulièrement sa branche ou son code avec la branche principale.
3. **Ne pas occulter un conflit** : le report à plus tard peut être plus gênant qu'autre chose.
4. **Commiter fréquemment** : moins de code modifié = moins de conflits possibles

