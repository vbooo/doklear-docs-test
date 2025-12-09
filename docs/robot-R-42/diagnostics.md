ROBOT AUTONOME R-42
02 · Diagnostic & dépannage
Ce guide fournit une procédure structurée pour diagnostiquer les problèmes les plus courants du robot R-42 : démarrage, réseau, capteurs, navigation et performances.

Introduction

Même après une mise en route correcte, un robot R-42 peut rencontrer des anomalies : impossibilité de se connecter à la console, trajectoires erratiques, messages d’erreur capteur, etc.

L’objectif de ce guide est de proposer une démarche de diagnostic simple, pour que le support de niveau 1 puisse qualifier le problème avant d’escalader vers l’équipe robotique.

Schéma global du robot R-42 et de ses sous-systèmes
Vue d’ensemble des principaux sous-systèmes du R-42 (alimentation, réseau, capteurs, navigation).
Prérequis

Le robot a été mis en route selon le guide Mise en route du robot.
Accès à la console R-42 avec un compte support.
Accès physique au robot si nécessaire (pour redémarrage ou inspection).
Mise en pratique

1. Le robot ne démarre pas

![Robot ne démarre pas](robot-no-working/carte.png)

Vérifier que le robot est correctement positionné sur la base de charge.
Maintenir le bouton d’alimentation pendant 5 secondes.
Observer le code couleur de la LED principale :
Rouge fixe : batterie trop faible → laisser charger 30 minutes.
Orange clignotant : erreur matérielle → vérifier l’écran de diagnostic.
2. Problème de connexion réseau

Schéma de connexion réseau du robot R-42
Exemple de topologie réseau typique : R-42 connecté au switch local puis à la console centrale.
Depuis la console, vérifier si le robot apparaît dans la liste des équipements.
Si absent, connecter un écran/clé USB au port de maintenance et vérifier l’adresse IP.
Tester un ping depuis un poste sur le même réseau : ping <ip_du_robot>.
En cas d’échec, repasser par l’interface locale (http://r42.local:8080) pour reconfigurer le réseau.
3. Erreurs capteurs (LiDAR / IMU / caméras)

Zone capteurs du robot R-42 vue de face
Exemples de zones à inspecter visuellement : fenêtre LiDAR, caméras frontales et capteurs de proximité.
Depuis la console, ouvrir la page Diagnostics > Capteurs.
Identifier le capteur en erreur (icône rouge ou orange).
Pour un LiDAR en erreur : vérifier visuellement qu’aucun film de protection ou poussière importante n’obstrue la fenêtre.
Lancer le test automatique du capteur. Si l’erreur persiste, collecter le rapport et créer un ticket niveau 2.
4. Navigation instable ou trajectoires incohérentes

Vérifier que la carte utilisée est bien la dernière version validée.

![Used mother  board](mother-board-used/carte.png)

Contrôler que le sol n’a pas été modifié (nouveaux obstacles fixes).
Lancer une routine de recalibrage IMU depuis la console (Maintenance > Calibrage).
Si le problème n’est présent que sur certaines zones, noter les coordonnées et le nom de la mission associée pour analyse ultérieure.
5. Performances dégradées

Consulter les journaux système sur les 24 dernières heures.
Vérifier l’utilisation CPU/GPU dans la section Monitoring.
S’assurer qu’aucune tâche de fond lourde (reconstruction de carte, update) n’est en cours pendant les missions.
Conclusion

Ce guide fournit une première ligne de diagnostic pour les incidents courants sur le robot R-42. Il permet de filtrer les problèmes simples (configuration, réseau, calibrage) avant de solliciter l’équipe d’ingénierie.

Pour tous les cas où la sécurité des opérateurs ou des infrastructures pourrait être engagée, se référer en priorité au guide 03 · Sécurité & bonnes pratiques.
