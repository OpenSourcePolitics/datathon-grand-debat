# Le grand débat sur Decidim
Analyse des données locales du grand débat émanant de l'instance Decidim de la Métropole Européenne de Lille (MEL).

La plateforme de démocratie participative libre et open source basées sur le logiciel libre [Decidim](https://decidim.org) pour proposer aux citoyens des modalités de débats plus ouvertes de contributions que le site officiel granddebat.fr. En effet le site officiel imposait de répondre à des questionnaires fermés ou publics, les utilisateurs pouvaient consulter les réponses pour ces derniers mais ne pouvaient pas commenter et échanger sur la plateforme.

Les citoyens ont ainsi pu contribuer de deux manières : 

- commenter les  questions du Président de la République communiquée dans sa [lettre au français](https://www.elysee.fr/emmanuel-macron/2019/01/13/lettre-aux-francais)
- déposer des contributions de manière totalement libre sur les 4 thématiques proposées Impôts, dépenses, action publique, Organisation de l’Etat et des collectivités publiques, Transition écologique, Démocratie et citoyenneté et Autres thématiques.
- les citoyens pouvaient également soutenir les propositions en votant

## Notre objectif
Analyser les données émanant de  cet exercice local pour qu'elles puissent être comparées à celle du site officiel et participer de la synthèse collective. Il sera intéressant de voir quel impact sur les contributions le fait de proposer des modalités de contributions plus ouvertes.

Si nous avons suffisamment le temps nous essayerons de comparer nos jeux de données avec ceux du granddebat.fr en les filtrant par département.

## Notre méthode d'analyse
Les corpus représentant déjà plusieus centaines de contributions nous allons utiliser dans notre travail des outils relevant du domaine du TAL (traitement automatique du langage). Ce domaine, situé au croisement de la linguistique, de l’informatique et de l’intelligence artificielle, offre un large panel de logiciels permettant d’enrichir la compréhension générique d’un grand ensemble de données textuelles tout en demeurant représentatif des spécificités et de la granularité du corpus. 

Tels que nous avions pu le faire pour la [synthèse de la consultation de l'Assemblée Nationale sur la démocratie numérique](http://www2.assemblee-nationale.fr/static/reforme-an/democratie/Rapport-democratie-2017-11-22.pdf) nous avons utilisé l’outil de textométrie [IRaMuTeQ](http://iramuteq.org/) pour obtenir un traitement rapide et précis du jeu de données complet qui nous a été remis par l’Assemblée nationale au lendemain de la clôture de la consultation en ligne. Ce logiciel libre développé par Pierre Ratinaud au sein du Laboratoire d’Etudes et de Recherches Appliquées en Sciences Sociales (LERASS) de l’université de Toulouse, propose un ensemble de méthodes statistiques pour réaliser notamment des nuages de mots, graphs de similitudes et tableaux d’analyse factorielle des correspondances. 

Pour plus d'info sur notre méthodologie lire la partie [I](https://medium.com/open-source-politics/pour-une-lecture-repens%C3%A9e-des-concertations-gr%C3%A2ce-au-traitement-automatique-des-langues-8d73977b0112?source=collection_home---4------0---------------------) et [II](https://medium.com/open-source-politics/les-innovations-m%C3%A9thodologiques-utilis%C3%A9es-par-osp-pour-lanalyse-des-discours-23a4165fbcfc?source=collection_home---4------1---------------------) de nos articles traitant du sujet.

## Les données
### Liens vers les concertations sur Decidim :
- [MEL](https://participation.lillemetropole.fr/processes/granddebatmel)
- [Nancy](https://participez.nancy.fr/processes/GrandDebatNational)

### Jeux de données :
MEL & Nancy
- Commentaires 30 questions 
- Propositions libres
  - Titre
  - Description
  - Catégorie
  - Commentaire  
  - Nombre de vote / soutien (juste pour la MEL)

