# O2Switch
https://dimitri-restaurant.simploncertif.fr/



Il dispose d’un cpanel, qui permet de créer des comptes messagerie, créer une base de données,  gérer les fichiers d’une application, d’un nom de domaine, l’installation d’un certificat ssl etc…  

Outre son coté illimité, il dispose d’un cpanel, qui permet de créer des comptes messagerie, créer une base de données,  gérer les fichiers d’une application, d’un nom de domaine, l’installation d’un certificat ssl etc…  

![Screenshot 2024-09-17 at 20.53.49.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/a7f63026-7145-47ac-81c0-4bd9e2123ad5/Screenshot_2024-09-17_at_20.53.49.png)

Procédure de déploiement : 

Pour déployer une application, vous devez d’abord  enregistrer un domaine préalablement acheté. 

![Screenshot 2024-09-17 at 20.57.15.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/531b9cd0-7f9e-4689-a917-8554e2068d89/Screenshot_2024-09-17_at_20.57.15.png)

Entrez le nom du domaine, la racine du document est l’endroit ou seront stocker les fichiers de votre application. 

Si vous avez besoin de créer une base de données,  retourner sur le cpanel et cliquez sur  assistant base de données mysql ( ou postgres  au besoin )

![Screenshot 2024-09-17 at 20.58.57.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/27290a0a-40db-44eb-8d87-60ff5f83eb73/Screenshot_2024-09-17_at_20.58.57.png)

Entrez le nom de votre futur base de données, et conservez le  pour lereporter dans votre fichier de connexion php.

![Screenshot 2024-09-17 at 20.59.31.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/2b62c61a-896d-4201-98a7-be15c1847bbb/Screenshot_2024-09-17_at_20.59.31.png)

Entrez ensuite un nom d’utilisateur que vous conserverez également, n’oubliez pas votre pseudo avant  exemple ici : nqws0790_test_deploiement

![Screenshot 2024-09-17 at 21.00.23.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/e96da5e6-2d1c-4ba9-a041-2e7764b9b23d/Screenshot_2024-09-17_at_21.00.23.png)

Cochez les droits que vous souhaitez donner à cet utilisateur

![Screenshot 2024-09-17 at 21.01.35.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/cae64cab-bf4c-4007-9e94-2435be5dc4c1/Screenshot_2024-09-17_at_21.01.35.png)

Cliquer sur apporter les modifications et vous aurez cet écran pour confirmer que vous avez créer la base de données. 

![Screenshot 2024-09-17 at 21.02.16.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/ceee31e0-ad97-4b9d-b3d4-84f8513410f8/Screenshot_2024-09-17_at_21.02.16.png)

Exporter votre bdd mysql en local, puis allez sur l’interface phpmyadmin du cpanel 

![Screenshot 2024-09-17 at 21.07.37.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/2dddd70d-01e9-4495-a30c-54fa0ac8ccdc/Screenshot_2024-09-17_at_21.07.37.png)

Selectionner à gauche la bdd que vous venez de créer, et importer votre fichier sql 

![Screenshot 2024-09-17 at 21.07.55.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/9ef4e00a-7d27-4da1-b509-04716234ce1d/Screenshot_2024-09-17_at_21.07.55.png)

et cliquez sur importer

![Screenshot 2024-09-17 at 21.08.50.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/46579dbf-f4f9-43c4-b62f-c73cd455f8b0/Screenshot_2024-09-17_at_21.08.50.png)

Si tout s’est bien passé, vous aurez un message comme ceci : 

![Screenshot 2024-09-17 at 21.09.08.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/dde6d565-9603-4db4-97ce-9a6956a861dd/Screenshot_2024-09-17_at_21.09.08.png)

et on peut voir les données comme ceci :

![Screenshot 2024-09-17 at 21.09.53.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/593f78f5-b95f-473d-8bfe-a58dff9f022e/Screenshot_2024-09-17_at_21.09.53.png)

Il ne nous reste plus qu’a importer notre fichier et nous connecter à la bdd

Modifier votre fichier pour intégrer vos identifiants de connexion à la bdd

![Screenshot 2024-09-17 at 21.15.17.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/2429cb2b-8caa-40be-838a-0a3490fd41bb/Screenshot_2024-09-17_at_21.15.17.png)

Retournez ensuite sur le cpanel  dans gestionnaire de fichiers

![Screenshot 2024-09-17 at 21.23.10.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/90835a00-ff8a-4d5a-b27c-5c88788b48ed/Screenshot_2024-09-17_at_21.23.10.png)

Vous retrouverez le nom d’un dossier au même nom que votre domaine ou sous domaine 

![Screenshot 2024-09-17 at 21.23.48.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/9fb78c83-262e-46af-ad97-80adc1ae7f11/Screenshot_2024-09-17_at_21.23.48.png)

Cliquez sur charger et uploadez vos fichiers

![Screenshot 2024-09-17 at 21.24.29.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/75486b78-6b56-4a22-99bd-831512854660/Screenshot_2024-09-17_at_21.24.29.png)

Success ! 

![Screenshot 2024-09-17 at 21.29.36.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/ac1c291b-4a63-40e2-b19d-441ef56623eb/Screenshot_2024-09-17_at_21.29.36.png)

En revanche, il vous faudra ajouter un certificat ssl avec let’s encrypt , retournez dans le cpanel , 

cliquez sur let’s encrypt  ssl 

![Screenshot 2024-09-17 at 21.30.26.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/a019409e-1ff3-4225-a955-dc9cebc373ef/Screenshot_2024-09-17_at_21.30.26.png)

Trouvez le domaine à configurer et cliquez sur Générer

![Screenshot 2024-09-17 at 21.31.09.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/49464fb5-90b3-47e5-9bcc-6abd491ea5e4/Screenshot_2024-09-17_at_21.31.09.png)

sur la page suivante, cliquez sur générer également.

![Screenshot 2024-09-17 at 21.31.41.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/3ad51a26-d562-47fe-bcd7-92db4d9d35f4/923fca8e-f049-4f3c-99be-151cc37cb642/Screenshot_2024-09-17_at_21.31.41.png)

Vous pourrez mettre également dans votre .htaccess, une redirection forcée en https , 
remplacer yourdomain par votre domaine# deploiement
