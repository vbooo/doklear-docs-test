# Ingestion de la documentation (version historique)

## Introduction
Cette procédure décrit l’ingestion “classique” utilisée par Doklear : la doc est découpée en chunks, puis indexée.
Utilisez cette méthode si votre documentation est principalement en Markdown et structurée par fichiers.

## Prérequis
- Ayez accès à un dépôt Git contenant vos guides.
- Vérifiez que vos fichiers sont en `.md` ou `.mdx`.
- Organisez vos dossiers par domaine fonctionnel (ex: `docs/auth/`, `docs/api/`, `docs/tutorials/`).

## Instructions
1. Connectez-vous à Doklear.
2. Cliquez sur **Ingestion**.
3. Sélectionnez l’onglet **GitHub**.
4. Collez l’URL de votre dépôt.
5. Renseignez la branche (ex: `main`).
6. (Optionnel) Renseignez un préfixe (ex: `docs/`).
7. Cliquez sur **Lancer l’ingestion**.
8. Attendez que le job passe en `success`.
9. Ouvrez la liste des documents et vérifiez que les titres sont corrects.

## Notes
- Si votre dépôt contient beaucoup de fichiers, commencez par un sous-dossier (préfixe).
- Évitez de mélanger doc produit et doc interne au même endroit si possible.

## Conclusion
Une fois l’ingestion terminée, lancez un audit pour détecter les problèmes de structure, de cohérence et de duplication.
Si vous observez des incohérences, ré-ingérez après correction des fichiers.
