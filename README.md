# O2Switch
https://dimitri-restaurant.simploncertif.fr/





Procédure de déploiement : 

Pour déployer une application, vous devez d’abord  enregistrer un domaine préalablement acheté. 


Entrez le nom du domaine, la racine du document est l’endroit ou seront stocker les fichiers de votre application. 

Créer une base de données,  retourner sur le cpanel et cliquez sur  assistant base de données mysql ( ou postgres  au besoin )


Entrez le nom de votre futur base de données, et conservez le  pour lereporter dans votre fichier de connexion php.


Entrez ensuite un nom d’utilisateur que vous conserverez également, n’oubliez pas votre pseudo avant  exemple  : nqws0790_test_deploiement


Cochez les droits que vous souhaitez donner à cet utilisateur


Cliquer sur apporter les modifications et vous aurez cet écran pour confirmer que vous avez créer la base de données. 


Exporter votre bdd mysql en local, puis allez sur l’interface phpmyadmin du cpanel 

Selectionner à gauche la bdd que vous venez de créer, et importer votre fichier sql 

et cliquez sur importer

Si tout s’est bien passé, vous aurez un message comme ceci : 

et on peut voir les données comme ceci :

Il ne nous reste plus qu’a importer notre fichier et nous connecter à la bdd

Modifier votre fichier pour intégrer vos identifiants de connexion à la bdd

Retournez ensuite sur le cpanel  dans gestionnaire de fichiers

Vous retrouverez le nom d’un dossier au même nom que votre domaine ou sous domaine 

Cliquez sur charger et uploadez vos fichiers

Success ! 

En revanche, il vous faudra ajouter un certificat ssl avec let’s encrypt , retournez dans le cpanel , 

cliquez sur let’s encrypt  ssl 

Trouvez le domaine à configurer et cliquez sur Générer

sur la page suivante, cliquez sur générer également.

Vous pourrez mettre également dans votre .htaccess, une redirection forcée en https , 
remplacer yourdomain par votre domaine# deploiement
