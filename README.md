
Réseau social
=============
Architecture dossier :
------------------------
* ### css

  *Ce dossier contient des feuilles de style personnalisées :*
    * styles.css
  
* ### filters

  *Ce dossier contient les fichiers de sécurité permettant de rediriger l'utilisateur,* 
  
  __(connecté) sera redirigé sur profil.php s'il tente d'accéder à:__
    * connexion.php
    * inscription.php
    
  __(déconnecté) sera redirigé sur connexion.php s'il tente d'accéder à:__
    * profil.php \+ tous les fichiers gérés par une session
    
* ### img

  *Contient toutes les images du site et des utilisateurs*
  
  
* ### inc
  
  *Contient un fichier config ainsi que le template du site*
  
    * init.inc.php
      * connexion à la base de donnée
      * démarrage de la session
      * inclusion du fichier *functions.php*
      * possibilité de réécrire ses chemins d'accès
    
    * functions.php
    
      *Permet d'écrire des fonctions*
      
    * haut.inc.php
    
      *Découpage du __\<\!DOCTYPE\>__ jusqu'à la __\<\/nav\>__ fermante du template*
      
    * bas.inc.php
    
      *Découpage de la __\<\/div\>__ fermante du container jusqu'à la balise fermante __\<\/html\>__*
    
* ### js

  *Contient tous les fichier .js*
  
  * main.js
  
    *Permet la liaison avec __search.php__ par l'intermédiaire de l'ajax*
  
* ### views

  *Permet de séparer la vue de la logique php*
    * __index.php__ => __index.view.php__
    * __profil.php__ => __profil.view.php__
    * __connexion.php__ => __connexion.view.php__
    * __inscription.php__ => __inscription.view.php__
    * __search.php__ => __search.view.php__
    * __amis.php__ => __amis.view.php__
    
