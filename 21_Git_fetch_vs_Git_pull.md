# quand utiliser git fetch ou git pull

git fetch et git pull sont deux commandes Git utilisées pour récupérer des mises à jour depuis un dépôt distant, mais elles ont des fonctionnalités différentes 

## Utilisation de git fetch 

### Quand l'utiliser ?

* Lorsque vous souhaitez récupérer les dernières modifications d'un dépôt distant sans fusionner automatiquement ces modifications avec votre travail local.
* Pour vérifier les mises à jour du dépôt distant sans impacter vos branches locales.
* Pour obtenir une vue d'ensemble des modifications avant de les fusionner manuellement dans votre branche.

### Avantages :

* Télécharge uniquement les données du dépôt distant dans votre dépôt local sans fusionner les modifications automatiquement.
* Vous permet de consulter les changements avant de les intégrer dans votre branche locale.

## Utilisation de git pull 

### Quand l'utiliser ?

* Lorsque vous souhaitez récupérer les dernières modifications du dépôt distant et les fusionner automatiquement avec votre branche locale.
* Pour synchroniser rapidement votre travail local avec le dépôt distant.

### Avantages :

* Télécharge les dernières modifications du dépôt distant et les fusionne automatiquement avec votre branche locale en une seule commande.
* Pratique pour une mise à jour rapide du travail local.


## Choix entre git fetch et git pull
* Si vous voulez seulement vérifier les modifications sans fusionner automatiquement : Utilisez git fetch.
* Si vous voulez récupérer les modifications et les fusionner immédiatement : Utilisez git pull.
* Pour une meilleure visibilité des changements avant de les fusionner : Utilisez git fetch suivi d'un examen des modifications récupérées avant de fusionner avec git merge ou git rebase.

**En résumé**, git fetch est plus sûr pour obtenir une vue d'ensemble des modifications avant de les intégrer, tandis que git pull est plus rapide et pratique pour récupérer et fusionner les modifications en une seule étape. Choisissez en fonction de votre flux de travail et de votre besoin spécifique à synchroniser votre dépôt local avec le dépôt distant.