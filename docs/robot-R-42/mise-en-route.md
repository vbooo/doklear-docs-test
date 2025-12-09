01 · Mise en route du robot
Ce guide explique comment mettre en service un robot autonome R-42 : vérifications matérielles, connexion au réseau et configuration initiale via la console.

Introduction

Le robot R-42 est un robot mobile indoor, équipé de capteurs LiDAR, de caméras RGB-D et d’une unité de calcul embarquée sous Linux. Il est conçu pour des tâches de patrouille, d’inventaire ou de transport léger en environnement structuré (entrepôt, usine, bâtiment tertiaire).

Avant de pouvoir l’utiliser dans un scénario réel, il faut passer par une phase de mise en route unique : enregistrement du robot, configuration réseau, mise à jour logicielle et premier calibrage des capteurs.

Prérequis

Un robot R-42 chargé à au moins 50 %.
Un point d’accès Wi-Fi ou un port Ethernet disponible dans la zone de test.
Un ordinateur portable avec un navigateur récent (Chrome, Firefox, Edge).
Les identifiants d’un compte administrateur sur la plateforme R-42 Console.
Mise en pratique

1. Vérifications matérielles

Contrôler visuellement l’état des bumpers, du LiDAR et des caméras.
Vérifier que l’interrupteur d’arrêt d’urgence est en position relevée.
Confirmer que la base de charge est correctement alimentée.
2. Connexion réseau

Allumer le robot à l’aide du bouton principal (LED passe au bleu fixe).
Connecter l’ordinateur portable au même réseau (Wi-Fi ou Ethernet).
Accéder à l’interface locale : http://r42.local:8080 ou l’adresse IP affichée sur l’écran du robot.
Dans l’onglet Network, sélectionner le réseau Wi-Fi de production et saisir la clé de sécurité.
3. Enregistrement sur la console

Ouvrir https://console.r42.local depuis le navigateur.
Se connecter avec un compte administrateur.
Cliquer sur Ajouter un robot puis scanner le QR code du R-42.
Attribuer un nom lisible (ex. : R42-Entrepot-A-01).
4. Mise à jour et calibrage de base

Depuis la console, aller dans Maintenance > Mises à jour et appliquer les mises à jour disponibles.
Lancer l’assistant Quick Calibration pour vérifier les capteurs LiDAR et IMU.
Effectuer un trajet simple en mode manuel pour valider la navigation de base.
Conclusion

À l’issue de ce guide, le robot R-42 est enregistré, à jour et connecté au réseau. Il est prêt à être intégré dans un scénario de mission plus avancé.

En cas de comportement anormal (problème de démarrage, messages d’erreur, navigation instable), se reporter au guide 02 · Diagnostic & dépannage.
