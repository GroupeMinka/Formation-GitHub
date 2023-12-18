# les Pull Request (PR)
Une "GitHub Pull Request" (PR) est une fonctionnalité d'interaction collaborative sur la plateforme GitHub. Elle permet à un contributeur de proposer des modifications à un dépôt et de solliciter la fusion (merge) de ces modifications dans la branche principale du projet. Les PR facilitent la revue de code, la discussion et la collaboration entre les membres d'une équipe travaillant sur un même projet.

## Étapes pour créer une Pull Request sur GitHub 

### 1. Créer une branche :
Avant de commencer à apporter des modifications, créez une branche distincte à partir de la branche principale du dépôt pour travailler sur votre fonctionnalité ou correction de bug.

### 2. Apporter des modifications :
Apportez les modifications nécessaires dans votre branche locale. Assurez-vous que ces modifications sont cohérentes et liées à un seul objectif (fonctionnalité, correction, amélioration, etc.).

### 3. Pousser la branche vers GitHub :
Une fois que vous êtes satisfait des modifications, poussez la branche vers GitHub en utilisant la commande git push.

### 4. Créer la Pull Request sur GitHub :

1.Allez sur la page principale du dépôt sur GitHub.
2.Cliquez sur l'onglet "Pull Requests" (ou "Pull requests" en anglais).
3.Cliquez sur le bouton "New pull request".
4.Sélectionnez la branche que vous avez poussée vers GitHub comme base de comparaison (base branch) et la branche principale du projet comme branche de comparaison (compare branch).

### 5. Soumettre la Pull Request :

1. Ajoutez un titre et une description décrivant les modifications apportées.
2. Si nécessaire, mentionnez des personnes spécifiques pour leur demander un examen (code review).
3. Cliquez sur le bouton "Create pull request" pour soumettre la PR.

### 6. Examiner et discuter des modifications :
Les autres membres de l'équipe peuvent maintenant examiner vos modifications. Ils peuvent commenter, poser des questions et suggérer des modifications via des discussions directement sur la PR.

### 7. Apporter des modifications et mettre à jour la PR :
Si des modifications sont nécessaires suite aux commentaires reçus, effectuez ces changements localement, poussez à nouveau votre branche et la PR sera automatiquement mise à jour.

### 8. Fusionner la PR :
Une fois que les modifications ont été approuvées et que tous les tests nécessaires sont passés, un mainteneur du dépôt peut fusionner la PR en cliquant sur le bouton "Merge pull request".

### 9. Supprimer la branche **(optionnel)** :
Après la fusion, vous pouvez supprimer la branche de votre dépôt local et distant si elle n'est plus nécessaire.