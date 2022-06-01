NB : En télechargeant directement l'archivre : https://github.com/Ardies-1001/facebook-api-login/
vous n'auriez simplemen qu'a l'installer et configurer vos accès d'application facebook

$fb = new Facebook\Facebook([
  'app_id' => '1214799411888113',
  'app_secret' => '286f08b36691768f859a70e788f4ceda',
  'default_graph_version' => 'v2.5',
]);
le package et autre dépendance sont déjà installé


Facebook offre une excellente alternative au processus de connexion traditionnel basé sur un formulaire 
qui fait depuis longtemps partie des applications PHP. L'idée est très simple; il vous suffit de mettre 
un bouton Facebook sur la page d'inscription. Ensuite, enregistrez les données utilisateur après une 
connexion réussie. 

je vais vous expliquer comment vous pouvez ajouter Facebook Login aux applications PHP 
et obtenir les données des utilisateurs

Comment se connecter avec Facebook via/en utilisant php ? 
Il se compose de seulement quatre étapes pour se connecter avec Facebook PHP SDK :

1- Créez une application Facebook.
2- Créez une application sur le serveur.
3- Téléchargez le SDK Facebook.
4- Comment puis-je initialiser PHP SDK sur Facebook et obtenir des informations sur l'utilisateur.

Détails

1 - Créer une application dans Facebook
Pour implémenter le système de connexion Facebook pour l'application, la première étape est la création d'une application via le compte Facebook

> Connectez-vous à Facebook et accédez à developer.Facebook.com .
> Cliquez sur le bouton Ajouter une nouvelle application et sélectionnez Site Web comme plate-forme.
> Entrez le nom de l'application, un identifiant de messagerie et sélectionnez une catégorie pour l'application. Cliquez maintenant 
	sur le bouton Créer un identifiant d'application. Cela créera une application sur Facebook.
> Allez maintenant dans Paramètres, où se trouvent le secret de l'application et l'ID de l'application. Ces identifiants 
	seront utilisés dans l'application PHP.  N'oubliez pas d'ajouter l'URL du site Web dans les domaines d'application.
> En bas de la page, cliquez sur l'onglet Ajouter une plate-forme. Ajoutez un site Web en tant que plate-forme et entrez l'URL du site Web.

Ceci termine la création de l'application Facebook. L'étape suivante consiste à créer un serveur sur une plate-forme d'hébergement rapide et fiable. 

2 - Créer une application sur le serveur

> Pour créer un serveur PHP , inscrivez-vous sur votre hébergeur et lancez un serveur PHP dessus.
> Visitez le serveur et lancez le terminal SSH. Connectez-vous à SSH à l'aide des informations d'identification principales.
> Accédez au dossier de l'application en exécutant la commande suivante
	$ cd applications/{your application folder}/private_html/
	
3 - Télécharger le SDK Facebook

Information :
	Composer est la méthode recommandée pour installer des bibliothèques sur la plate-forme et je l'utiliserai pour installer
	le SDK Facebook. La première étape consiste à créer un fichier de composition. Dans le terminal SSH, exécutez la commande 
	composer init et ajoutez-y les informations requises. Il créera un fichier composer.json dans le dossier de l'application. 
	Ajoutez le code suivant dans composer.json.
	
Exécutez maintenant la commande composer install dans SSH pour finaliser l'installation du SDK Facebook.

4 - Comment puis-je initialiser PHP SDK sur Facebook et obtenir des informations sur l'utilisateur

> Il est maintenant temps d'initialiser le SDK Facebook et d'obtenir access_token de Facebook. Après avoir authentifié le jeton, 
les informations de l'utilisateur seront récupérées et la vue sera redirigée vers la page de profil qui affiche 
les informations de l'utilisateur.

> Créez deux fichiers dans le dossier de l'application : Index.php et Profil.php.

> Le code source des pages profil.php et index.php est disponible avec des commentaires ajoutés.

> Une fois cela fait, accédez à l'URL de l'application dans le navigateur. Vous verrez le bouton 
	Facebook pour vous connecter. Cliquez dessus et la page sera redirigée vers la page de connexion 
	Facebook. Connectez-vous au compte Facebook. Après une connexion réussie, la page sera redirigée 
	vers la page de profil.

> Ajoutez le code suivant à profile.php pour afficher les informations récupérées. Pour les besoins 
	de ce tutoriel, je vais récupérer l'identifiant de l'utilisateur, la photo de profil Facebook, 
	le nom et l'e-mail.

Conclusion
j'ai montré comment intégrer le bouton Facebook Login dans vos applications PHP. 
Cela éliminera les tracas liés au remplissage et à l'analyse de longs formulaires d'inscription. 
Si vous avez besoin de poser une question sur le code , écrivez moi sur : lebonadjanohoun7@gmail.com


