# Claynum — Périmètre et responsabilités

Version initiale — document de travail évolutif.

## Objectif

Ce document définit ce que Claynum peut réaliser directement, les domaines dans lesquels Claynum peut accompagner le client, et les sujets qui nécessitent l’intervention d’un spécialiste.

L’objectif est d’éviter les attentes implicites, de limiter les zones grises et de conserver des solutions proportionnées au besoin réel.

## Légende

- **Fait** : Claynum peut prendre en charge directement la réalisation ou la configuration dans un périmètre simple et défini.
- **Accompagne** : Claynum peut cadrer, conseiller, comparer des solutions, préparer ou réaliser une partie de la mise en œuvre, sans se substituer au spécialiste responsable du domaine.
- **Spécialiste requis** : sujet hors du périmètre de responsabilité de Claynum ; orientation vers un professionnel compétent.

## Matrice de périmètre

| Domaine | Fait | Accompagne | Spécialiste requis / limites |
|---|---|---|---|
| Cadrage d’un besoin numérique | Oui | — | — |
| Analyse d’un processus simple | Oui | — | — |
| Proposition d’une solution proportionnée | Oui | — | — |
| Choix entre outil existant et développement spécifique | Oui | — | — |
| Site vitrine statique | Oui | — | — |
| Petite application web métier | Oui, selon complexité | Oui | Architecture complexe ou forte criticité à cadrer séparément |
| Application poste de travail simple | Oui, selon besoin | Oui | Déploiement massif ou environnement complexe hors périmètre initial |
| Base de données simple | Oui | — | Haute disponibilité, volumétrie importante ou données fortement sensibles à cadrer avec un spécialiste |
| Formulaire métier / tableau de suivi | Oui | — | — |
| Automatisation simple | Oui | — | Automatisation critique ou à forte dépendance métier à cadrer séparément |
| Reprise / simplification d’un outil existant | Oui | Oui | Selon technologie et dette technique |
| Nom de domaine | Accompagnement au choix, à la disponibilité et à l’enregistrement | Oui | Le domaine et le compte registrar restent au nom et sous la maîtrise du client ; le client reste responsable du renouvellement |
| DNS courant | Oui : configuration A, AAAA, CNAME, MX, TXT, redirections et vérifications usuelles | Oui | Architecture DNS complexe ou critique, split-DNS, infrastructure d’entreprise, haute disponibilité ou cas DNSSEC avancé : spécialiste |
| Hébergement Web léger | Oui | Oui | Hébergement critique, haute disponibilité, PRA/PCA : spécialiste |
| Hébergement infogéré simple | Non en exploitation permanente | Oui | Exploitant/hébergeur responsable du service |
| Certificat TLS / HTTPS | Oui, cas standard | Oui | PKI complexe ou certificats internes : spécialiste |
| Messagerie professionnelle | Oui, paramétrage simple | Oui | Administration avancée, migration volumineuse ou sécurité renforcée : spécialiste |
| Microsoft 365 / suites bureautiques | Paramétrage simple | Oui | Gouvernance tenant, sécurité avancée ou migration importante : spécialiste/intégrateur |
| Sauvegarde | Mise en place simple | Oui | Stratégie de sauvegarde critique, PRA/PCA ou contraintes réglementaires : spécialiste |
| MFA / gestion simple des accès | Oui | Oui | IAM complexe, fédération d’identité, SSO d’entreprise : spécialiste ou intégrateur dédié |
| Gestion des droits applicatifs simples | Oui | — | Modèle d’habilitation complexe à cadrer avec le client |
| Sécurité de base d’un petit SI | Oui, recommandations et configuration simple | Oui | Audit de sécurité formel, pentest, homologation ou certification : spécialiste |
| Audit de sécurité / pentest | Non | — | Spécialiste cybersécurité requis |
| Supervision 24/7 | Non | — | Exploitant ou prestataire spécialisé requis |
| Astreinte / support permanent | Non | — | Hors périmètre initial |
| Maintenance applicative ponctuelle | Oui, si prévue au cadrage | Oui | Pas d’engagement implicite de support permanent |
| Formation utilisateur ciblée | Oui | — | Formation certifiante ou réglementée : organisme compétent |
| Formation numérique adaptée au besoin | Oui | — | Périmètre à définir avec le client |
| Sélection de logiciels SaaS | Non comme revendeur | Oui | Contrat souscrit directement par le client |
| Comparaison des coûts numériques | Oui | — | Tarifs à vérifier au moment de la décision |
| RGPD — identification des points d’attention | Non comme conseil juridique | Oui | Le client reste responsable de traitement ; DPO ou juriste si nécessaire |
| RGPD — mise en œuvre technique | Oui, si simple | Oui | Validation juridique hors périmètre |
| Cookies / traceurs | Oui, mise en œuvre technique | Oui | Qualification juridique du consentement : CNIL/DPO/juriste si doute |
| Mentions légales | Non comme rédacteur juridique | Oui | Validation juridique par le client ou un professionnel compétent |
| Politique de confidentialité | Non comme conseil juridique | Oui, mise en forme / intégration technique | Rédaction/validation juridique : DPO ou juriste |
| Registre des traitements | Non comme responsable de conformité | Oui, aide à structurer les informations | Validation DPO/juriste selon contexte |
| Contrats | Non | — | Avocat / juriste |
| Statuts de société | Non | — | Avocat, expert-comptable ou formaliste compétent |
| Fiscalité | Non | — | Expert-comptable / administration fiscale |
| Comptabilité | Non | — | Expert-comptable |
| Droit social | Non | — | Juriste / avocat / expert compétent |
| Applications mobiles avec publication sur stores | À évaluer | Oui | Publication, conformité store et maintenance à cadrer séparément |
| Infrastructure cloud complexe | Non en première intention | Oui pour le cadrage | Architecte / intégrateur cloud selon besoin |
| Haute disponibilité | Non | Oui pour expression du besoin | Spécialiste infrastructure |
| SI critique ou réglementé | Non en responsabilité globale | Oui pour cadrage limité | Intégrateur / RSSI / DPO / spécialiste selon domaine |

## Principes de fonctionnement

1. **Partir du besoin réel** avant de choisir une technologie ou un produit.
2. **Privilégier l’outil existant** lorsqu’il répond correctement au besoin.
3. **Développer uniquement ce qui apporte une valeur concrète** et identifiable.
4. **Éviter le surdimensionnement** : ne pas faire payer aujourd’hui une architecture destinée à un besoin hypothétique futur.
5. **Préserver l’évolutivité raisonnable** : une solution simple ne doit pas créer volontairement une impasse.
6. **Rendre explicites les limites de responsabilité** avant le démarrage de la prestation.
7. **Ne pas se substituer à un juriste, un expert-comptable, un DPO, un RSSI ou un autre spécialiste** lorsque le sujet dépasse le périmètre numérique opérationnel de Claynum.
8. **Documenter les dépendances externes** : hébergeur, SaaS, bibliothèque, API, licence et coût récurrent.
9. **Le client conserve la maîtrise de ses comptes et abonnements** : domaine, hébergement, licences et services doivent autant que possible être souscrits en son nom.
10. **Pas d’astreinte implicite** : support, maintenance et disponibilité doivent être explicitement prévus lorsqu’ils sont nécessaires.

## Utilisation future

Cette version est destinée au cadrage interne. Une version client pourra être simplifiée en trois colonnes :

- Claynum prend en charge ;
- Claynum accompagne ;
- spécialiste nécessaire.

Le document doit évoluer à partir des missions réellement rencontrées et des limites techniques, juridiques ou organisationnelles constatées.