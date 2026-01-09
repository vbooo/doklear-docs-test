# Ingestion de la documentation (nouvelle version / migration)

## Introduction
Cette page décrit la nouvelle ingestion “V2” : Doklear analyse davantage la structure et rapproche les contenus par concepts.
Utilisez cette version si vous avez une documentation plus hétérogène (HTML, fichiers, Git, fragments).

## Prérequis
- Connectez au moins une source de doc (GitHub ou URL).
- Vérifiez que vos pages HTML sont accessibles sans authentification (ou configurez un accès).
- Préparez un périmètre clair (ex: doc publique uniquement).

## Instructions
1. Connectez-vous à Doklear.
2. Ouvrez **Ingestion**.
3. Choisissez la source (GitHub ou URL).
4. Lancez l’ingestion.
5. Ouvrez ensuite l’onglet **Search** et vérifiez que vos concepts clés sont retrouvables.
6. Lancez un audit et vérifiez les alertes “structure” et “obsolescence”.

## Différences par rapport à la version historique
- Les documents sont regroupés par **concepts dominants** (ex: “auth”, “billing”, “API keys”).
- Doklear rapproche les guides similaires pour détecter des divergences.
- Les sections sont utilisées pour améliorer la navigation (citations vers section).

## Conclusion
Si vous migrez depuis l’ancienne ingestion, conservez les anciens guides pendant une période de transition.
Doklear vous aidera à identifier ceux qui deviennent à risque d’obsolescence (drift avec les nouveaux guides).
