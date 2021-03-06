# 03/01/2021

- Ajout de la possibilité de changer la source depuis un scénario (via une liste déroulante) 
- Correction de l'icône Afficheur On/Off dans le widget de la V4

# 30/05/2020

- MAJ du template mobile (mieux vaut tard que jamais !)
- Correction d'un bug dans l'état (play/pause)
- Ajout d'un label mute à côté de l'état dans le template (dashboard et mobile)

# 17/05/2020

- Séparation du cron principal en deux crons : 
  - un cron pour les infos du player,
  - un cron dédié uniquement à son état (Etat Power)
- Correction de l'info Etat Power qui ne se mettait pas à jour (PWON ou PWSTANDBY)
- Ajout des commandes (Telnet classique) On et Off

# 16/05/2020

- Refonte de la partie favoris (récupération dynamique du SID de la station dédiée aux favoris)
- Correction du démon pour ne mettre à jour les infos que du players concerné lorsqu'il y a plusieurs enceinte configurées dans le plugin

### **ATTENTION : La mise à jour concernant les favoris nécessite de rééxectuer la commande "Récupérer le PID" sur chaque équipement (si vous souhaitez utiliser les favoris)**

# 13/05/2020

- Ajout de la possibilité de chercher le PID par nom (en plus de l'IP car pour certains modèles, l'IP ne remonte pas forcément depuis l'API HEOS dans le résultat de recherche)
- Correction mineures

# 05/10/2019

- Ajout de la possibilité de lancer un favoris depuis un scénario (commande *Jouer un favoris*, voir documentation)

# 03/07/2019

- Ajout d'une commande Power avec comme choix possible On ou Off
- Passage sur la modale du core jeedom à la place de la modale custom (modale favoris + groupe)
- Optimisations mineures

# 29/06/2019

- Correction et amélioration dans la gestion des groupes
- Correction d'un bug lors de l'arrêt de l'appareil qui affichait un titre dans certains cas
- Correction de la mise à jour de l'état au démarrage d'une lecture qui resté sur stop dans certains cas
- Augmentation de la taille des icônes d'action secondaire (favoris, groupe, luminosité...)

# 28/06/2019

- Ajout d'une commande **Luminosité** permettant de choisir une luminosité via une liste déroulante (0%, 25%, 50%, 75% ou 100%). A utiliser par exemple dans un scénario ou sur un widget perso (non dispo sur le widget du plugin). Pour les players type AVR, seul trois niveaux de luminosité existent, les niveaux 75% et 100% sont donc identiques.
- Optimisation de code

# 19/06/2019

- Passage de la modale des favoris sur une modale de même type que celles de jeedom (évite les interférences avec le css du core de jeedom)
- Ménage dans la solution (suppression des dossiers inutiles)
- Ajout de la traduction en_US (90%)

# 16/06/2019

- Correction de l'affichage de la modal des favoris lorsque le widget est utilisé dans un design jeedom.
- Ajout de la récupération du modèle dans la configuration de l'équipement
- Prise en compte du modèle pour les deux commandes annexes loudness et luminosité (nécéssite de récupérer à nouveau le PID avec le bouton dédié dans la configuration de l'équipement)
- Divers ajustements graphiques

# 15/06/2019

- Correction pour éviter le lancement en double de la connexion telnet lors du lancement du daemon
- Ajout de la possibilité de renseigner son compte HEOS dans la configuration de l'équipement (login + mot de passe, nécessaire pour l'utilisation de certaines fonctions comme les Favoris HEOS)
- Ajout de la possibilité de consulter et de lancer un favoris Heos (icône étoile en haut à droite du widget)

# 12/06/2019

- Correction du widget pour prise en compte de la couleur de fond en fonction de la catégorie choisie pour l'équipement
- Refresh auto du widget à l'enregistrement de l'équipement

# 11/06/2019

- Ajout de la récupération auto du PID du player à l'adresse IP renseignée
- Définition des valeurs du widget par défaut à l'enregistrement de l'équipement (titre, album, artiste, image)

# 10/06/2019

- Alignement des textes à gauche (titre, album, artiste)
- Ajout de la documentation
- Correction de la gestion de l'allumage ou non de l'afficheur (le toogle était inactif si la valeur choisie par défaut dans la configuration de l'équipement était différente de 100%)
- Ajout d'un toogle pour activation/désactivation du loudness
- Sélection par défaut de l'image blanche et de la luminosité à 25%

# 09/06/2019

- Version initiale
