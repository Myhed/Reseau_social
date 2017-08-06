# Réseau Social
## Architecture des dossiers

* ### css

  *Ce dossier contient des feuilles de style personnalisées ici :*
    * style.css

* ### filters

  *Ce dossier contient les fichiers de sécurité permettant de rediriger l'utilisateur si
	il est déjà connecter ou déconnecter :*

	__Sera rediriger sur membre.php si il tente d'accéder à (Connecté):__
    * Connexion.php
    * Inscription.php

	__Sera rediriger sur connexion.php si il tente d'accéder à (Déconnecté) :__
    * membre.php \+ tous les fichiers gérant une session

* ### img

  *Contient tous les images du site et des utilisateurs*
* ### inc

  *Contient un fichier config ainsi que le template du site
    * init.inc.php
    
      __Permet :__
        * connexion à la base de donnée
        * démarage de la session
        * Inclusion du fichier fonctions.php
        * Possibilité de réecrire ses chemins d'accés
        
    * functions.php
    
      *Permet d'écrire des fonctions*
      
    * haut.inc.php
    
      *Découpage du __DOCTYPE__ jusqu'à la __\<\/nav\>__ (fermante)*
      
    * bas.inc.php
    
      *Découpage de la __\<\/div\>__ du container jusqu'à la balise __\<\/html\>__ (fermante)*
* ### js
  *Ce dossier contient tous les fichiers js*
  
    * main.js
      *Permet la liaison avec __search.php__ par l'intermédiaire de l'ajax*
      
* ### views

  *Permet de séparer la vue de la logique php*
  
    * __index.php__ => __indew.view.php__
    * __connexion.php__ => __connexion.php__
    * __membre.php__ => __membre.view.php__
    * __searchView.php__ => __search.view.php__
    * __amis.php__ => __amis.view.php__

