# Devis express

Prototype d'outil pour les installateurs en **plomberie, pompes à chaleur et énergies renouvelables** : il génère un devis à partir d'un type d'installation et prépare des relances clients automatiques.

> **Statut : prototype (v0.1).** Il sert à valider le besoin auprès d'artisans, pas à être utilisé en production.

## Ce que fait le prototype

- Choix du type d'installation : PAC air/eau, climatisation réversible air/air, chaudière gaz à condensation, chauffe-eau thermodynamique, plancher chauffant, photovoltaïque 3 kWc.
- Lignes de devis pré-remplies, modifiables (désignation, quantité, prix), avec ajout et suppression de lignes.
- Calcul automatique du total HT, de la TVA (5,5 %, 10 % ou 20 %) et du total TTC.
- Options : contrat d'entretien annuel, visite technique préalable.
- Trois messages de relance prêts à copier (après 3, 7 et 15 jours), mis à jour avec le client, le projet et le montant.
- Copie du devis en texte, impression ou export PDF via le navigateur.
- Thème clair et sombre selon l'appareil.

## Lancer le projet

Aucune installation : c'est un seul fichier HTML sans dépendance (hors police Google Fonts, avec repli sur les polices système).

1. Télécharge ou clone le dépôt.
2. Ouvre `index.html` dans ton navigateur.

### Mettre en ligne avec GitHub Pages

1. Crée un dépôt sur GitHub et envoie les fichiers.
2. Dans **Settings > Pages**, choisis la branche `main` et le dossier `/ (root)`.
3. Le site est disponible à l'adresse `https://<ton-compte>.github.io/<nom-du-depot>/`.

## Limites connues

- **Les prix sont des exemples**, sans valeur réelle. Chaque installateur doit renseigner ses propres tarifs.
- **La TVA et les aides publiques (MaPrimeRénov', CEE, éco-PTZ) ne sont pas calculées** et doivent être vérifiées par l'installateur avant d'envoyer un devis.
- Aucune sauvegarde : les données sont perdues à la fermeture de la page.
- Pas de signature électronique, pas d'envoi par mail, pas de numérotation légale des devis.
- Le devis généré est un **brouillon** : mentions légales obligatoires, assurance décennale et conditions de vente sont à ajouter selon l'activité.

## Pistes d'évolution

- [ ] Enregistrer le catalogue de prix de chaque artisan (stockage local, puis base de données).
- [ ] Devis généré à partir d'une note vocale ou d'un formulaire de visite technique.
- [ ] Envoi des devis et des relances par mail ou SMS, avec suivi des réponses.
- [ ] Génération des documents de fin de chantier (attestations, rapports d'intervention).
- [ ] Préparation des pièces des dossiers d'aides, sans promesse de montant.
- [ ] Connexion aux logiciels de facturation existants.

## Données et conformité

Le prototype ne stocke ni n'envoie aucune donnée. Une version réelle manipulera des données personnelles de clients : prévoir le RGPD (contrat de sous-traitance, durée de conservation, hébergement en Europe).

## Contribuer

Les idées, retours d'installateurs et propositions sont les bienvenus via les *issues* du dépôt.

## Licence

À définir par l'auteur avant publication (par exemple MIT pour un projet ouvert, ou « tous droits réservés » si tu veux garder le code privé).
