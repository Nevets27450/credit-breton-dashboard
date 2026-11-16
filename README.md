# Crédit Breton — Tableau de bord Power BI

Rapport d’analyse des demandes de prêt, des profils emprunteurs et de l’activité des agences bretonnes.

## Contenu

- Page d’accueil et présentation du rapport.
- Vue d’ensemble des demandes et financements.
- Analyse des demandes de prêt.
- Performance et carte des agences.
- Analyse des clients et détail des demandes.

## Ouvrir le projet

1. Installer une version récente de Power BI Desktop compatible PBIP/PBIR.
2. Ouvrir `Credit Breton.pbip`.
3. Dans **Transformer les données → Gérer les paramètres**, renseigner `CheminSource` avec le chemin du classeur source.
4. Actualiser les données.

Le classeur doit contenir les feuilles **Demandes de pret**, **Agences**, **Situation pro**, **Apport** et **Situation famille**, avec les colonnes attendues par les requêtes Power Query. Les données sources et caches locaux ne sont pas distribués dans ce dépôt.

## Indicateurs

Demandes reçues, clients distincts, taux d’accord, financement demandé et accordé, délai de clôture. Le taux d’accord exclut les demandes sans décision. Le financement accordé ne représente pas un décaissement. Les règles emprunteur sont indicatives et distinctes des décisions enregistrées.

## Structure

- `Credit Breton.pbip` : point d’entrée du projet.
- `Credit Breton.Report/` : pages, visuels et ressources graphiques.
- `Credit Breton.SemanticModel/` : tables, relations, mesures DAX et requêtes Power Query.

## Carte

La carte Azure Maps nécessite une connexion Internet et l’activation du visuel dans Power BI. Les coordonnées proviennent du classeur source. Le contour de Bretagne est fourni par [france-geojson](https://github.com/gregoiredavid/france-geojson), sous licence [MIT](https://github.com/gregoiredavid/france-geojson/blob/master/LICENSE).
