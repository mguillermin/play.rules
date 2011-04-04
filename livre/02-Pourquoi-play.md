# Pourquoi Play

Play framework est une vraie révolution dans le monde des application Web écrites en Java. Il vous fera oublier toutes les souffrances que vous avez pu vivre avec la pile Java EE classique, des frameworks comme Spring ou pire, J2EE.
Architectures techniques opaques, gestion chaotique des dépendances, longues phases de compilation, redémarrage du serveur à chaque modification du code... tout ça ne sera bientôt pour vous que de mauvais souvenirs :)

    TODO détailler chaque point
    

## Architecture simple

Play se base sur une architecure extrêment simple en suivant le design pattern MVC. A côté de ça il ne rajoute pas de notions de couches service, couches DAO etc.
Tout le code métier est porté par les objets du modèle, comme préconisé dans la méthode de conception [DDD](http://fr.wikipedia.org/wiki/Conception_pilot%C3%A9e_par_le_domaine) (domain driver design).
Comme en Ruby On Rails, les objets du modèle sont conçus selon le pattern Active Record : ils ont la capacité de gérer eux même leur persistence dans la base de données.

On peut par exemple écrire le code suivant pour manipuler une entité "Personne" : 

    //Si on voulait récupérer toutes les personnes
    //List<Personne> personnes = find("byName","Dupont");
    //Récupérer la personne ayant l'id 1
    Personne p1 = Personne.findById(1);
    //Modification de l'entité
    p1.firstName = "paul";
    //Mise à jour dans la base de données
    p1.save();

## Orienté REST
    TODO URL "bookmarkables" et explicites : chaque page est une ressource 

## Stateless et scalable


##Productif (convention over configuration, hot deploy, CRUD...)

## Extensible (modules)

## Pur Java

## Java tricks (encapsulation ...)

## Exemples
    TODO détailler ces exemples http://www.playframework.org/documentation/1.0/5things