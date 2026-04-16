## Activer la persistance sur notre application

Une difficulté avec le cluster IP que j'avais oublié de mettre à None ce qui empêchait le statefulset de fonctionner. De ce que j'ai compris c'est parce que l'on ne veut pas que le service associé au statefulstate ait une IP unique fixe ce qui pourrait poser des problèmes justement pour la persistence mais plutôt des IPs pour les pods.

Erreur aussi parce que mon formatter à l'enregistrement ne sait pas bien gérer les identations en yaml (:

Finalement ça fonctionne ! Mes données persistent maintenant :))

## Quel est l'intérêt du StatefulSet par rapport au Deployement ? 

Le StatefulSet est utile quand les applications ont besoin de garder un état stable avec des noms fixes et un stockage persistant pour chaque instance. Le Deployment est plutôt fait pour des applications où les pods peuvent être créés/supprimés sans importance ce qui offre plus de flexibilité et scalabilité.