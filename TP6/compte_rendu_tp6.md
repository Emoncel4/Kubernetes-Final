## Création d'un secret pour stocker le user et le password de la bdd 

Assez simple quand on regarde comment fonctionne les secrets. Juste à faire bien attention à enlever les informations sensibles de la configmap et à bien relier le secret au statefulset. Le seul problème demeure le fait que tout supprimer et tout relancer reste pour l'instant le seul moyen d'être sûr que tout fonctionne (ou non). J'ai l'impression que relancer uniquement ce qui me semble nécessaire parvient rarement au résultat escompté.

## Mise en place d'un init container

J'ai eu des problèmes pour identifier les colonnes de la base de données et j'ai dû rentrer dans les logs du pod pour voir pourquoi le post ne fonctionnait pas depuis le frontend.

Note : je n'ai pas refaite les probes ici car déjà traitées au TP5 et je préférais repartir sur la base avec l'image docker fournie au TP3. 