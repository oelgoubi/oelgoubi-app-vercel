# OelgoubiApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.0.5.

# Question 4 : 
  vercel -v
# Question 5 : créer un projet Angular via la commande :
  ng new oelgoubi-app

# Question 6 : Déployer l'application dans vercel 
  vercel deploy

# Question 7 : lister les différents déploiements
   vercel ls

# Question 8 : afficher les logs liés au déploiement précédent
  vercel logs oelgoubi-app-q46r8wkfk.vercel.app

# Question 9 : La commande inspect sert à afficher les informations relatives à un déploiement
    Pour l'utiliser , on peut passer l'url unique du déploiment :
    vercel inspect oelgoubi-app-q46r8wkfk.vercel.app

# Question 10 :
 Les Varibales d'environnement sont généralement utilisées pour définir la configuration d'un application, par exemple : rensigner la configuration d'une base de données ( nom d'utilisteur , mot de passe et le nom de la base de donnée) ou des TOKENS qui nous permettent  de consommer une API. Donc l'objectif est de séparer la configuration requise par un environnement de production de celle requise par un environnement de développement.

# Question 11 : créer une variable d'evironnement et renseigner sa valeur.
  vercel env add plain MY_VAR production
# Question 12 : lister les variables d'environnement sur le projet
  vercel env ls

# Question 13 : 
La commande "vercel secrets" est utilisée pour gérer les secrets utilisés dans les variables d'environnement, les secrets sont des informations sensibles que nous voudrions protégées.


# Question 15 : Créez une variable d'env de type secret
  vercel secrets add MYSQLDB_PASS mysqldbPass213

# Question 16 : Les trois environnements que vercel nous met à diposition sont : 
- Développement 
- Preview (environnement de prévisualisation ou pré-production)
- Production 

On cherche à isoler les environnements les uns des autres tant que possible, pour plusieurs raisons :
- Chaque environnement a un but précis, requiert des performances,des données et des utilisateurs précises.
6 
 -L'environnement de développement est utilisé tout au long de la phase de développement de   l'application ( développement d’une ou plusieurs fonctionalités et des tests associés )
 -L'environnement de pré-production est un environnement intermédiaire utilisé après le développement  , et avant la mise en production, il nous permet d'obtenir des résultats de tests pertinents.
 -L'environnement de production est utilisé par les clients, il doit rester disponible sur les plages horaires prévues,fournir un accés sécurisé en HTTPS et il supporte un traffic important.


# Question 18 :  https://oelgoubi-app-vercel-v2.vercel.app/

# Question 19:
Un pull request est une fonctionalié qui permet de faciliter la collaboration entre les développeurs qui travaillent sur le même projet , il est en fait une demande de pull (ajout) d'un code au répertoire faite par un memebre de l'équipe. Le code produit peut servir à corriger certains bugs ou l'ajout des nouvelles fonctionalités à l'application. Les autres collaborateurs doivent analyser ces changement , les tester et ensuite les intégrer au projet.

Aprés la création de mon pull request, vercel a bien pris mes changements en compte et il a déployer l'application dans un environnement de pré-production et finalement, il m'a fournit un lien pour accéder à l'application, voir les changements pour les valider avant de les intégrer dans le code dédié à l'environnement de production.

# Question 20 :
Une foit la pull request a été fusionné avec la branche master , vercel l'a détécté et il a redéployer l'application dans l'environnement de production.

# Question 21 :
- L'environnement de production correspond à la branche master

- L'intéret d'utiliser des pull requests sur un projet est de analyser le code produit par chaque membre de l'équipe de développement , le tester puis le valider avant de l'intéger au code du projet.
Ils permettent aussi de déclencher les processus de déploiment gérés par vercel.

- Dans 


# BONUS : inspect nous permet d'inspecter l'appli une fois déployé , et logs nous permet de voir les logs qui ont été générés lors du processus de déploiment.