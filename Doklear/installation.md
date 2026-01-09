# Installation de Doklear (SaaS)

## Introduction
Doklear est disponible en SaaS. Vous n’avez rien à installer côté serveur.
Configurez simplement un workspace et connectez votre documentation.

## Prérequis
- Ayez accès à un compte Doklear.
- Préparez une documentation source :
  - dépôt Git (Markdown),
  - pages web (HTML),
  - ou fichiers (PDF, MD, TXT).

## Instructions
1. Connectez-vous à votre compte Doklear.
2. Sélectionnez votre workspace dans le menu (en haut).
3. Ouvrez l’onglet **Ingestion**.
4. Choisissez une source :
   - **GitHub** : collez l’URL du dépôt.
   - **URL** : collez une liste de pages à ingérer.
   - **Fichiers** : uploadez un PDF ou du Markdown.
5. Lancez l’ingestion et attendez que le job passe en `success`.
6. Ouvrez l’onglet **Audit**.
7. Lancez un audit en mode **trial** (ou full si activé).

## Conclusion
L’installation SaaS consiste essentiellement à connecter une source et lancer l’audit.
Vous pouvez ensuite brancher le widget sur votre site pour capturer de vraies questions d’utilisateurs.
