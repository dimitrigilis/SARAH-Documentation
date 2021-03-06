# FAQ / Résoudre un problème

Si vous ne trouvez pas de réponses dans cette communauté
- Regarder dans la FAQ lié à votre version de SARAH [v3](faq_v3) ou [v4](faq_v4)
- Chercher de l'aide sur le [groupe Google+](http://community.sarah.encausse.net).


## Sommaire

## Projet SARAH

### Pourquoi SARAH ?

- Le projet a été créé en 2012 issue d'une idée datant de 2007.
- Le nom du projet est tiré de [la série TV Eureka](http://www.syfy.com/eureka/). 
- Son nom signifie: _Self Actuated Residential Automated Habitat_
- L'objectif du projet était:
  - D'apprendre les technologies NodeJS et C#
    - Le Computer Vision 
    - Kinect
  - De découvrir l'Internet des Objets
  - D'apprendre le Community Management

SARAH est un projet couteux et chronophage soyez indulgent !

### Un projet OpenSource ?

J'ai l'habitude de partager mes développements sous la forme [d'articles](http://encausse.net) et [code source](https://github.com/JpEncausse), si cela peut aider...

Les sources de SARAH sont sur GitHub sous licence [WFTPL](fr.wikipedia.org/wiki/WTFPL).
- La [Documentation](https://github.com/JpEncausse/SARAH-Documentation)
- SARAH v3 [Client](https://github.com/JpEncausse/WSRMacro) et [Server](https://github.com/JpEncausse/WSRNodeJS) 
- SARAH v4 [Client](https://github.com/JpEncausse/SARAH-Client-Windows) et [Server](https://github.com/JpEncausse/SARAH-Server-NodeJS)

Le projet est organisé sous la forme de plugins développés par la communauté. Je ne prends pas de pull request car je n'ai pas le temps de coordoner des développements.

### Un Framework pas un Produit ?

SARAH n'est pas un produit clef en main. C'est un Framework permettant d'interragir avec les objet connectés. 
- Pour les gens techniques, curieux, bidouilleurs, ...
- Pour tester et inventer de nouveaux usages entre les objets connectés, avec la famille, la maison, ...

Il faut voir ce projet comme un outil pour prototyper la maison connectée tout comme le propose Arduino sur l'électronique. 


### Pour les enteprises ?

Les entreprises font ce qu'elles veulent la license est [WFTPL](fr.wikipedia.org/wiki/WTFPL). Mais il me semble dangereux de monter un business sur un projet codé au fond du garage.

SARAH n'est pas un produit car:
- Les gens ne sont pas prêt à payer
- L'architecture est dépendante de Windows
- Un produit implique une ergonomie bien plus simple
- un produit implique beaucoup de maintenance et de support

Par contre j'ai la structure pour organiser des Hachathons autour de SARAH financés par les entreprises qui le souhaitent. Il m'est aussi possible d'aider sur la conception d'un plugin. 

### Comment aider SARAH ?

SARAH était un des premiers projet de maison intelligente. 

- Parlez de SARAH http://sarah.encausse.net autour de vous, sur les réseaux sociaux, dans les medias, etc ...
- Parlez de votre expérience avec SARAH, faites des vidéos de vos installations c'est très précieux !
- Participez à la documentation, développez des plugins, ...
- Vous pouvez me [faire un don](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=H9ALBBSZFL6CU) si vous le souhaitez
- Entreprises, vous pouvez m'envoyer vos objets connectés pour réaliser un POC de plugin.

### Futur de SARAH ? 

En réponse à un [post sur Google+](https://plus.google.com/u/0/+ChristopheGardelle/posts/HBbQoYNEqyT?cfem=1), le créateur de SARAH nous en apprend plus sur le futur de celle-ci : 
- la v5 est en préparation et sera disponible via https://github.com/NGRP/node-red-contrib-viseo
- « la v5 ne sera pas compatible avec la v4/v3 mais la philosophie reste la même et donc le code assez simple à porter »
- la v5 est opensource mais sponsorisée par l'entreprise VISEO

Le développement de la v3 et de la v4 sont donc arrêtés.

### Le Store ne fonctionne pas ! Où trouver et comment installer les plugins ?

La machine qui héberge le store de SARAH n'est plus fonctionnelle et il est possible que le store ne soit pas remis en état... Cependant la plupart des plugins peuvent être trouvés et téléchargés sur Github : https://github.com/search?utf8=%E2%9C%93&q=SARAH-Plugin&type=

Pour installer un plugin, télécharger le contenu du compte Github associé puis placer le contenu dans le répertoire `plugins` de votre installation de SARAH.

### Où télécharger SARAH ?

Vous pouvez trouver les dernières releases sur ce compte Github : https://github.com/JpEncausse/SARAH-Documentation/releases

### Quelles langues parle SARAH ?

SARAH supporte toutes les langues du moteur de reconnaissance vocale de Microsoft.
- L'application web SARAH v3 est en Anglais
- L'application web SARAH v4 est multilangue en Anglais et Français
- Les plugins sont essentiellement en Français de par la communauté

## HardWare

### Quelles sont les objets compatibles SARAH ?

- Il y a plus de 200 plugins sur le [marketplace](/home?page=marketplace)
- De manière général tous les objets qui ont une API (cherher sur GitHub)

### Quelle configuration machine ?

Le client SARAH necessite **une machine windows**.
- La reconnaissance vocale consomme 10% d'un CPU Core i5 de NUC
- La reconnaissance gestuelle / faciale consomme 40% d'un CPU Core i5 de NUC

Configuration atypiques:
- Le serveur NodeJS peut tourner sur un Raspberry Pi.
- Certaines personnes ont virtualisé SARAH sur Mac.
- Certaines personnes font tourné SARAH sur un NAS.

### Quel micro prendre: Kinect 1 ou Kinect 2 ?

Le Kinect [est bien meilleur](http://blog.encausse.net/2013/05/19/thevoice/) pour la reconnaissance vocale, et fournit aussi des fonctionnalités supplémentaires (_gesture, face recognition, QRCode, ..._).
Si vous voulez utiliser SARAH avec un Kinect, merci de lire les informations ci-dessous :
* Kinect v1 pour XBox 360
  * Environ 50€ (rechercher sur LeBonCoin à 30€)
  * Il doit être fourni avec le câble USB et l'alimentation
  * D'après la licence il ne peut être utilisé que par les développeurs (c'est donc le cas avec SARAH)
* Kinect v1 pour Windows
  * Plus cher
* Kinect v2 pour XBox One
  * Environ 150€ (rechercher sur LeBonCoin à 80€)
  * Il doit être fourni avec le câble USB et l'alimentation
  * Acheter **en plus** un adaptateur Windows (50€ sur le Microsoft Store)
* Kinect v2 pour Windows
  * Environ 200€
  * Doit être installé sous **Windows 8.1** et doit utilisé de l'**USB 3**

### Peut-on utiliser plusieurs micros ?

La réponse est très dépendante de la version de SARAH:

- SARAH prends l'entrée d'un microphone 
- Il est possible d'utiliser plusieurs Kinect 1 sur un PC
- Il **n'est pas** possible d'utiliser plusieurs Kinect 2 sur un PC
- SARAH peut recevoir un flux RTP (d'un Raspberry Pi) comme microphone
- SARAH ne sait pas écouter les Cameras IP ou Interphones


### Peut-on utiliser plusieurs speaker ?

La réponse est très dépendante de la version de SARAH:

- SARAH parle sur les speaker par defaut
- Certains speaker bluetooth ont une veille / latence qui mange le début des phrases de SARAH
- Des logiciels comme  [Airfoil](https://www.rogueamoeba.com/airfoil/) stream avec de la latence sur des speaker AirPlay ou DNLA
- SARAH ne sait pas parler sur les Cameras IP ou Interphones

### Peut-on faire du Multiroom ?

- Une solution est de mettre plusieurs micros et plusieurs speakers.
- Les extentions USB/RJ45 Kinect ne marchent QUE pour l'Audio du Kinect 1.
- Il est possible d'avoir plusieurs clients SARAH.
- La communauté a développé des clients iOS, Android et Windows Phone.
- Il est possible d'utiliser [Mumble](http://www.mumble.com/) pour [connecter SARAH à plusieurs tablettes dans la maison](http://youtu.be/-lJT_I68Qk4).

### Est ce que SARAH existe sur Mobile ?

Oui le client Mobile discute avec le client SARAH
- Pour [Android](https://play.google.com/store/apps/details?id=net.android.clientsarah).
- Pour iOS sur la communauté
- Pour Windows Phone en beta sur la communauté

## Installation

Si ça ne marche pas regardez les logs du client ou du serveur qui donneront des indices de pourquoi ça ne marche pas. C'est souvent lié à un chemin de fichier, un port utilisé, un logiciel qui utilise les même ressources que SARAH.

### J'ai une erreur EADDRINUSE

L'erreur EADDRINUSE signifie "Error Address already In Use". Le port du serveur 8080 (or 8888 pour le client) déjà utilisé par un autre processus. Cela peut être un server SARAH mal fermé.

Utiliser la commande DOS `netstat` pour lister les ports utilisés.

### J'ai une erreur avec la DLL 'KinectAudio10.dll'

Si dans Log2Console vous obtenez l'erreur `Init Kinect Engines: impossible de charger la dll 'KinectAudio10.dll'` c'est que vous avez probablement installé une [version N de Windows](http://windows.microsoft.com/en-us/windows-8/upgrade-to-n). Pour y remédier, il faut installer un *Media Feature Pack*.

Exemple avec le [Media Feature Pack pour les versions N et KN de Windows 10](https://www.microsoft.com/fr-FR/download/details.aspx?id=48231) (pour Windows 10 avant Novembre 2015), ou encore [Media Feature Pack pour les versions N et KN de Windows 10 #2](https://www.microsoft.com/fr-FR/download/details.aspx?id=49919) (pour Windows 10 mis à jour après Novembre 2015), ou [Media Feature Pack pour les versions N et KN de Windows 10 #3](https://www.microsoft.com/en-us/download/details.aspx?id=53356) (pour Windows 10 mis à jour après le 1er août 2016), ou [Media Feature Pack pour les N et KN de Windows 10 Anniversary](https://support.microsoft.com/en-us/help/4016817/media-feature-pack-for-n-edition-of-windows-10-version-1703-april-2017) (pour Windows 10 mis à jour après le 1er avril 2017).

### Commment changer la voix de SARAH ?

Relire la documentation ➔ Configuration ➔ Synthèse Vocale dans laquelle il y a des références vers des voix et le lien vers l'interface de configuration 32bit. 

- Utiliser l'interface 64bit annulera la config 32bit
- Certaines voix trouvées sur internet plantent

### Comment supprimer un profil de reconnaisse vocale ?

Ce n'est pas toujours bon d'avoir suivi le tutoriel de reconnaissance vocale trop souvent. Si SARAH ne vous comprend plus correctement vous pouvez essayer d'effacer votre profil de reconnaissance vocale :    
Aller dans `Panneau de Configuration` ➜ `Reconnaissance Vocale` ➜ `Options vocales avancées` ➜ `Profils de reconnaissance vocal` ➜ `Supprimer...`

### SARAH v3 ne fonctionne toujours pas... comment trouver le problème ?

Plusieurs pistes qui peuvent aider à trouver le problème :

  1. Revérifier toutes les étapes d'installation (voir ["Premiers Pas pour la v3"](http://jpencausse.github.io/SARAH-Documentation/?page=getting_started_v3)).
  2. Ouvrir la page [http://127.0.0.1:8888/?emulate=Sarah+il+est+quelle+heure](http://127.0.0.1:8888/?emulate=Sarah+il+est+quelle+heure) : SARAH devrait vous donner l'heure. 
  3. Dire : "Sarah quelle heure est-il ?" et voir dans la console du serveur (la fenêtre DOS) s'il est marqué `"info: Run time: 10ms"`
  4. Sur l'icône de la maison (près de l'horloge de Windows) faire un clic droit puis choisir "Log2Console". Essayer ensuite de dire une phrase comme "Sarah quelle heure est-il ?" et vous devriez voir un certain nombre d'informations. Vous pouvez aussi laisser `log2console` ouvert pendant que vous redémarrez Sarah car des informations de déboggage y apparaissent également.  
  ![Ouvrir log2console](https://raw.githubusercontent.com/JpEncausse/SARAH-Documentation/gh-pages/markdown/images/log2console_click_house.png)   
  ![Dans log2console](https://raw.githubusercontent.com/JpEncausse/SARAH-Documentation/gh-pages/markdown/images/log2console_example.png)   
  5. Activer les logs (se reporter à la [configuration de la v3](http://jpencausse.github.io/SARAH-Documentation/?page=getting_started_v3#custom-ini)) dans `custom.ini` avec `debug=true` et `log=${basedir}/${shortdate}.log`, puis redémarrer SARAH. Essayer de nouveaux les étapes 2 et 3 ci-dessus et voir si un fichier de log apparait dans le répertoire `bin/` (vous y trouverez de possibles messages d'erreurs) et si un fichier `.wav` apparait dans le répertoire `dump` (si oui c'est que SARAH vous entend)
  5. Vérifier vos firewall et antivirus (en les désactivant temporairement par exemple)
  
Enfin poster le résultats de vos tests sur le [groupe Google+](https://plus.google.com/u/0/communities/105964514508504667709).
  
## Software

### Le serveur affiche une erreur

Si il y a une erreur de la forme `module not found` alors il y a une erreur dans le module. Contacter son auteur.

### SARAH devient sourde

Un plugin DOIT appeler son callback `next()` ou `callback()` pour indiquer au client que le travail est terminé. Sinon le client attends plusieurs minutes juqu'a un timeout.

SARAH n'écoute pas quand elle parle. Si le client plante a ce moment elle devient sourde ! Regardez et envoyez moi les logs du client !


