# Compte rendu du TP1

## Exercice 1

Pas de difficulté particulière pour les premières questions si ce n'est des problèmes de chemins vers les fichiers et les dossiers. J'ai repris la structure du dockerfile de ce site : https://docs.docker.com/get-started/docker-concepts/building-images/writing-a-dockerfile/. Et puis j'ai cherché comment lancer un dockerfile (*sudo docker build -t nom .*). J'ai eu un problème de Dockerfile que j'avais nommé DockerFile et qui donc ne voulait pas se lancer. (https://docs.docker.com/get-started/docker-concepts/building-images/build-tag-and-publish-an-image/)
Ensuite j'ai lancé l'image avec *sudo docker run -p 8080:8080 api-python*. Le get avec /hello fonctionne bien et renvoie "world". 
Les logs s'envoient bien dans mon terminal.
Pour le push j'ai d'abord dû créer un compte et le relier à ma machine. Je eu des problèmes car j'étais déjà connecté à un autre compte en parallèle qu'on avait utilisé dans le cadre d'un projet mais cela n'était pas indiqué. J'ai taggué mon image puis un *sudo docker push* a suffi.


## Exercice 2

Le deuxième exercice est très similaire au premier. J'ai simplement adapté le code en allant chercher récupérer les informations des slides du cours. J'ai modifié la version de java de façon à être conforme avec le pom.xml. La grande différence est le fait qu'il y a une compilation d'abord puis un run de l'appli.
Je n'ai pas refait les erreurs de chemins et de nommage du fichier cette fois-ci.