**CLAYNUM**

## Référentiel technique

Doctrine, périmètre et pratiques opérationnelles

**DOCUMENT INTERNE DE RÉFÉRENCE**

Version 1.0 — 14 août 2026

*Révision prévue après la passe de conception des schémas*

**Sommaire**

*Les chapitres suivent le cycle de vie d’une prestation, de la qualification du besoin à la réversibilité.*

# 1. Objet du référentiel

# 2. Doctrine d’intervention de Claynum

# 3. Qualification initiale du besoin

# 4. Niveaux d’intervention

# 5. Identité numérique et noms de domaine

# 6. Système de noms de domaine — DNS

# 7. Messagerie professionnelle

# 8. Hébergement et publication

# 9. Sites web

# 10. Applications sur mesure

# 11. Données et bases de données

# 12. Sécurité minimale applicable

# 13. Données personnelles et conformité

# 14. Déroulement d’une prestation

# 15. Exploitation, maintenance et assistance

# 16. Propriété, accès et réversibilité

# 17. Matrice des responsabilités

# 18. Modèles et annexes opérationnelles

# 1. Objet du référentiel

## 1.1 Finalité du document

Le présent référentiel fixe la doctrine technique et opérationnelle de Claynum. Il sert à qualifier les demandes, choisir un niveau d’intervention proportionné, définir les responsabilités et préparer les documents contractuels. Il constitue le point de départ des propositions, devis, fiches de cadrage, procès-verbaux de recette et documents de remise au client.

Le référentiel n’est ni un catalogue commercial ni un contrat type. Une prestation n’est engagée qu’après définition écrite de son périmètre, de ses livrables, de ses délais et de ses limites. En cas de contradiction, le document contractuel signé pour la prestation prévaut.

> **POSITION CLAYNUM**  
> Claynum cherche d’abord à résoudre un besoin concret. La solution technique doit rester compréhensible, proportionnée au contexte du client et exploitable sans dépendance artificielle au prestataire.

## 1.2 Public concerné

Le document est destiné en priorité :

- à Claynum, pour préparer et conduire les prestations de manière cohérente ;
- aux partenaires techniques ou spécialisés auxquels une partie du travail pourrait être confiée ;
- aux clients, lorsque la communication d’un extrait facilite la compréhension du périmètre ;
- aux conseils juridiques, comptables, assurantiels ou spécialisés sollicités sur un point précis.

Les clients visés sont principalement des indépendants, micro-entreprises, très petites entreprises, associations et structures locales dont les besoins numériques peuvent être couverts sans infrastructure complexe ni exploitation permanente.

## 1.3 Périmètre des prestations Claynum

Le périmètre de principe comprend :

- le diagnostic et la reformulation d’un besoin numérique ;
- l’accompagnement relatif aux noms de domaine, au DNS, à la messagerie et à l’hébergement ;
- la création ou l’amélioration de sites vitrines ;
- la conception d’applications web, de bureau ou de prototypes mobiles ;
- la création et l’utilisation de bases de données de complexité maîtrisée ;
- la mise en service, la documentation et le transfert de compétences ;
- une maintenance ponctuelle ou récurrente, expressément définie.

Sont exclus par défaut : l’astreinte, l’exploitation 24 h/24, la supervision de sécurité permanente, les audits réglementaires, l’hébergement en propre, l’administration générale du parc informatique du client et les projets dont la sensibilité ou la criticité dépasse les capacités d’une petite structure de prestation.

## 1.4 Documents auxquels il sert de référence

Le référentiel alimente notamment :

- la fiche de qualification initiale ;
- la proposition de solution ;
- le devis ou la lettre de mission ;
- le dossier de conception ;
- le plan de recette ;
- la fiche de mise en production ;
- le dossier de remise et de réversibilité ;
- le contrat ou l’avenant de maintenance.

## 1.5 Mise à jour et versionnement

Le document comporte un numéro de version et une date. Une évolution majeure du périmètre, de la doctrine, d’un socle technique ou d’une obligation réglementaire entraîne une nouvelle version. Les ajustements rédactionnels sans effet sur le fond peuvent être regroupés dans une révision mineure.

Les informations juridiques, réglementaires et de sécurité sont vérifiées périodiquement auprès de sources institutionnelles. Elles donnent un cadre de travail mais ne remplacent pas l’avis d’un professionnel compétent lorsque l’enjeu le justifie.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Place du référentiel dans le cycle d’une prestation Claynum  
> Objectif : montrer comment le référentiel alimente le cadrage, le devis, la réalisation, la recette et la remise  
> Éléments : besoin client, référentiel, documents contractuels, réalisation, validation, réversibilité  
> Type : flux documentaire

# 2. Doctrine d’intervention de Claynum

## 2.1 Le numérique comme moyen

Une demande formulée en termes d’outil ne décrit pas toujours le besoin réel. « Il me faut une application » peut en pratique signifier : centraliser une information, éviter une double saisie, suivre une échéance ou produire un document fiable. Claynum revient donc à l’activité, aux utilisateurs et au résultat attendu avant de choisir une technologie.

Cette approche évite de reproduire dans un nouvel outil un processus mal défini ou inutilement complexe. Elle permet aussi de reconnaître qu’un formulaire, un tableau correctement structuré ou une amélioration de l’organisation peut parfois suffire.

## 2.2 Proportionner la solution au besoin réel

La sophistication n’est pas une qualité en soi. Le choix d’une architecture doit prendre en compte :

- le nombre d’utilisateurs ;
- la fréquence d’utilisation ;
- la volumétrie des données ;
- la criticité du service ;
- les compétences disponibles chez le client ;
- le budget initial et les coûts récurrents ;
- la durée de vie probable de la solution.

Une solution locale ou statique peut être préférable à une plateforme complexe lorsqu’elle couvre correctement le besoin. À l’inverse, un service manipulant des données sensibles ou indispensable à l’activité exige des moyens d’exploitation et de sécurité que Claynum ne doit pas sous-estimer.

## 2.3 Privilégier les solutions simples et maintenables

Claynum recherche des composants connus, documentés et soutenus. Les dépendances sont limitées à ce qu’elles apportent réellement. Les choix techniques doivent pouvoir être expliqués et repris par un autre intervenant compétent.

La maintenabilité repose notamment sur :

- une structure de code lisible ;
- un historique de versions ;
- des paramètres séparés du code ;
- des secrets exclus du dépôt de code ;
- des procédures de déploiement et de restauration ;
- une documentation proportionnée ;
- des tests sur les fonctions importantes.

## 2.4 Distinguer les formes d’intervention

Le verbe employé engage le périmètre. Claynum distingue :

| Niveau | Signification | Exemple |
|---|---|---|
| Conseiller | présenter des options et leurs conséquences | comparer deux solutions d’hébergement |
| Accompagner | guider le client pendant une action qu’il réalise ou valide | créer un compte registrar au nom du client |
| Configurer | effectuer un réglage sur un service existant avec autorisation | ajouter un enregistrement DNS |
| Réaliser | produire un livrable défini | développer un site vitrine |
| Exploiter | assurer dans la durée le fonctionnement convenu | appliquer des mises à jour selon un contrat de maintenance |

Une prestation de conseil n’emporte pas exploitation. Une mise en service n’implique pas une surveillance permanente. Une aide ponctuelle ne crée pas une obligation générale de support.

## 2.5 Conserver au client la maîtrise de ses actifs

Sauf nécessité particulière explicitement acceptée, le client doit être titulaire :

- du nom de domaine ;
- des contrats d’hébergement et de messagerie ;
- des comptes de mesure d’audience ;
- des comptes de publication ;
- des espaces de stockage contenant ses données ;
- des moyens de paiement associés à ces services.

Claynum peut disposer d’un accès nominatif ou délégué limité au temps et au besoin de la prestation. Les comptes partagés et les abonnements souscrits durablement au nom du prestataire sont évités.

## 2.6 Développement assisté par intelligence artificielle

Les outils actuels de développement assisté par l’intelligence artificielle permettent aujourd’hui de réaliser plus rapidement certaines applications sur mesure. Claynum les utilise comme un accélérateur de réalisation, en gardant la maîtrise technique de ce qui est produit, de son fonctionnement et de sa cohérence avec le besoin.

Le recours à ces outils ne dispense jamais :

- de comprendre le code et l’architecture retenus ;
- de vérifier les dépendances et leurs licences ;
- de tester les fonctions importantes ;
- de contrôler les erreurs, les biais et les propositions inadaptées ;
- de protéger les secrets et données du client ;
- de documenter les choix structurants.

Les données confidentielles, personnelles ou métier ne sont pas transmises à un service d’IA sans base contractuelle, paramétrage approprié et accord explicite lorsqu’il est requis.

## 2.7 Limites générales de responsabilité

Claynum est responsable des prestations qu’il accepte dans les limites définies par le contrat. Le client reste responsable de ses décisions métier, du contenu qu’il publie, des instructions qu’il donne, des utilisateurs qu’il autorise et des obligations propres à son activité.

Les fournisseurs tiers restent responsables de leurs services selon leurs propres contrats. Claynum ne garantit pas l’absence de panne d’Internet, de l’hébergeur, du registrar, de la messagerie ou d’une API externe.

## 2.8 Prestations exclues ou soumises à un spécialiste

Une réorientation ou un partenariat spécialisé est requis pour les activités suivantes, sauf compétence et assurance ultérieurement établies :

- audit de cybersécurité ou test d’intrusion ;
- réponse à incident grave et investigation numérique ;
- conseil juridique, fiscal ou comptable ;
- hébergement de données de santé ou autres données soumises à un régime particulier ;
- systèmes industriels, objets connectés critiques ou équipements de sécurité physique ;
- services nécessitant une haute disponibilité contractualisée ;
- intégration de paiement ou commerce électronique complexe ;
- publication dans les magasins d’applications mobiles, hors prestation spécifique ;
- administration complète d’un système d’information ou support utilisateurs permanent.

> **POINT DE VIGILANCE**  
> Refuser ou réorienter une demande ne signifie pas qu’elle est techniquement impossible. Cela signifie que son niveau de risque, de criticité ou d’exploitation dépasse le cadre accepté par Claynum.

# 3. Qualification initiale du besoin

## 3.1 Activité, organisation et interlocuteurs

La qualification commence par l’activité réelle du client : ce qu’il produit, vend ou organise, les personnes concernées et les difficultés observées. Un interlocuteur décisionnaire et, si nécessaire, un référent métier sont identifiés.

La disponibilité du client est un facteur de réussite. Un projet ne peut pas être mené uniquement à partir d’une idée générale sans arbitrages, exemples, contenus ni validation régulière.

## 3.2 Objectif recherché

L’objectif est formulé comme un résultat observable. Par exemple :

- présenter clairement l’activité et permettre une prise de contact ;
- réduire le temps de saisie d’une information ;
- disposer d’une liste fiable et exportable ;
- suivre l’avancement d’un dossier ;
- automatiser la production d’un document répétitif ;
- permettre l’accès à une information depuis plusieurs appareils.

Les critères de réussite sont définis avant la réalisation. Ils doivent être compréhensibles sans référence à la technologie choisie.

## 3.3 Utilisateurs et volumes prévisionnels

La fiche de qualification recense :

- le nombre d’utilisateurs actuels et prévisionnels ;
- leur localisation et leurs équipements ;
- les rôles et droits nécessaires ;
- la fréquence d’utilisation ;
- le volume initial de données ;
- la croissance probable ;
- les périodes de pointe éventuelles.

Ces informations permettent d’éviter aussi bien le sous-dimensionnement que l’architecture disproportionnée.

## 3.4 Données et niveau de sensibilité

Les données sont classées au minimum selon quatre niveaux : public, interne, personnel courant, sensible ou réglementé. La présence de données de santé, d’informations financières détaillées, de données relatives à des infractions, de secrets d’affaires ou de données concernant des personnes vulnérables impose une analyse renforcée.

Lorsque le niveau de sensibilité est incompatible avec les moyens disponibles, Claynum limite le périmètre, propose une solution adaptée par un tiers ou refuse la prestation.

## 3.5 Contraintes réglementaires ou métier

Le client signale les obligations propres à son activité : conservation de documents, secret professionnel, réglementation sectorielle, exigences contractuelles, accessibilité, facturation, archivage ou localisation des données.

Claynum peut aider à traduire une exigence identifiée en mesure technique. Claynum ne détermine pas seul le droit applicable et ne valide pas juridiquement la conformité globale de l’activité.

## 3.6 Équipement et services existants

L’existant est inventorié avant de proposer un remplacement : domaine, messagerie, site, hébergeur, outils métiers, fichiers, bases de données, sauvegardes, comptes administrateurs et prestataires en place. Les dépendances et contrats à conserver sont identifiés.

## 3.7 Budget, délais et coûts récurrents

Le budget doit intégrer le coût initial et les dépenses récurrentes : abonnements, nom de domaine, hébergement, licences, stockage, envoi de courriels, API, maintenance et renouvellements. Un service gratuit peut être retenu, mais son modèle économique, ses limites et sa réversibilité doivent être compris.

Les délais dépendent autant de la disponibilité des contenus et validations que du temps de réalisation technique.

## 3.8 Identification des risques

La qualification relève au minimum :

- l’indisponibilité tolérable ;
- la perte de données acceptable ;
- l’existence d’une solution de repli ;
- la dépendance à un fournisseur ;
- la difficulté de reprise par un tiers ;
- le risque d’erreur humaine ;
- le risque d’accès non autorisé ;
- les conséquences d’un arrêt du projet.

## 3.9 Décision de prise en charge

À l’issue de la qualification, Claynum choisit l’une des positions suivantes :

1. prise en charge dans le périmètre standard ;
2. prise en charge avec réserves ou prérequis ;
3. intervention limitée à un diagnostic ou à un prototype ;
4. intervention conjointe avec un partenaire ;
5. réorientation ou refus motivé.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Arbre de décision de prise en charge d’une demande  
> Objectif : rendre visible le passage du besoin exprimé à la décision d’intervention  
> Éléments : besoin, sensibilité, criticité, compétences, budget, prise en charge, partenariat, refus  
> Type : arbre de décision

# 4. Niveaux d’intervention

## 4.1 Conseil

Le conseil apporte une analyse, des options et une recommandation. Le livrable peut être oral pour une demande simple ou formalisé dans une note lorsque la décision engage un coût, un risque ou une architecture.

Le client reste décisionnaire. Lorsqu’un choix repose sur une information fournie par le client, cette dépendance est indiquée.

## 4.2 Accompagnement

L’accompagnement vise à rendre le client autonome ou à lui permettre de rester titulaire de ses comptes. Claynum peut partager l’écran, préparer les informations, contrôler les réglages et expliquer les conséquences. Le client effectue ou valide les actions structurantes : souscription, paiement, acceptation de conditions générales, transmission d’une pièce d’identité ou choix d’un titulaire.

## 4.3 Configuration

La configuration est une modification effective d’un service existant. Elle suppose :

- une autorisation claire ;
- un accès adapté et temporaire si possible ;
- une sauvegarde ou un relevé de l’état initial ;
- une trace de la modification ;
- un contrôle après intervention ;
- une procédure de retour arrière lorsque l’enjeu le nécessite.

## 4.4 Réalisation

La réalisation produit un livrable : site, application, script, base de données, modèle ou documentation. Le périmètre fonctionnel, les hypothèses, les interfaces, les environnements cibles et les critères de recette sont définis.

Le développement par itérations permet de montrer tôt une version utilisable et d’éviter une incompréhension découverte en fin de projet.

## 4.5 Mise en service

La mise en service comprend les opérations explicitement prévues : déploiement, configuration de production, vérifications, sauvegarde initiale, contrôle des accès et remise d’un état de référence. Elle ne transforme pas automatiquement Claynum en exploitant permanent.

## 4.6 Formation et transfert

La formation porte sur les usages nécessaires au périmètre livré. Elle peut prendre la forme d’une démonstration, d’une séance guidée, d’une fiche pratique ou d’un guide d’administration.

Le transfert inclut les éléments nécessaires à la continuité : accès, code source convenu, inventaire, procédures et points de vigilance.

## 4.7 Maintenance ponctuelle

Une intervention ponctuelle répond à une demande identifiée et fait l’objet d’une estimation ou d’un accord spécifique. Elle n’implique ni surveillance continue ni délai garanti pour les demandes futures.

## 4.8 Maintenance récurrente

La maintenance récurrente nécessite un accord écrit précisant :

- les composants couverts ;
- les opérations prévues ;
- la fréquence ;
- le canal de demande ;
- les plages de disponibilité ;
- les délais indicatifs ou garantis ;
- les exclusions ;
- les conditions de sortie.

## 4.9 Prestations non assurées implicitement

Ne sont jamais déduits d’une intervention antérieure : l’astreinte, la sauvegarde permanente, la surveillance des journaux, la réponse immédiate à une panne, la restauration garantie, la veille réglementaire du client ou la prise en charge de tout nouveau besoin.

> **POSITION CLAYNUM**  
> Chaque prestation doit avoir un début, une fin et des livrables identifiables. Une relation durable est possible, mais elle repose sur un cadre de maintenance explicite et non sur une disponibilité informelle.

# 5. Identité numérique et noms de domaine

## 5.1 Choix du nom de domaine

Le nom de domaine doit être lisible, facile à dicter, cohérent avec l’activité et suffisamment distinctif. Les variantes principales peuvent être examinées afin de limiter les confusions, sans multiplier inutilement les achats.

Le nom de domaine n’est pas une marque. Avant un usage professionnel, la disponibilité doit être appréciée au-delà de la seule réponse du registrar : noms d’entreprises, marques, enseignes, usages antérieurs et risques de confusion. Une recherche simple ne vaut pas analyse juridique de disponibilité.

## 5.2 Vérification de disponibilité

Claynum peut vérifier la disponibilité apparente d’un domaine et aider à interpréter les informations publiques. La disponibilité reste susceptible d’évoluer jusqu’à l’enregistrement effectif.

Pour les domaines en .fr, les ressources de l’Afnic permettent de comprendre les rôles du registre, du bureau d’enregistrement et du titulaire. Pour d’autres extensions, les règles du registre concerné s’appliquent.

## 5.3 Choix du registrar

Le choix prend en compte :

- le prix d’enregistrement et de renouvellement ;
- la clarté de l’interface ;
- la protection du compte par authentification multifacteur ;
- la gestion DNS proposée ;
- la facilité de transfert ;
- la qualité du support ;
- les options ajoutées automatiquement ;
- les conditions de récupération du compte.

Le prix promotionnel de la première année ne doit pas masquer le tarif de renouvellement.

## 5.4 Enregistrement et renouvellement

Le compte est créé au nom et avec les coordonnées du client. Le client accepte les conditions du registrar et règle directement les frais. Claynum peut guider l’opération et vérifier le résultat.

Le renouvellement automatique est recommandé lorsque les moyens de paiement et alertes sont correctement tenus à jour. Une vérification périodique reste nécessaire. Le guide pratique de l’Afnic rappelle qu’il convient de contrôler les conditions de renouvellement même lorsqu’un mécanisme automatique est prévu.

## 5.5 Titularité du domaine

Le client doit être le titulaire réel du domaine. Les coordonnées doivent être exactes et accessibles. Claynum ne devient pas titulaire pour simplifier temporairement une procédure.

Les accès d’administration, l’adresse de récupération et l’authentification multifacteur doivent rester maîtrisés par le client. Un accès délégué à Claynum peut être créé lorsque le registrar le permet.

## 5.6 Extensions et redirections

L’achat de .fr et .com peut être pertinent pour une activité française, mais n’est pas systématique. Une extension principale est choisie ; les autres domaines redirigent vers elle. Les contenus dupliqués sur plusieurs domaines sont évités.

## 5.7 Protection minimale du compte

Le socle comprend :

- un mot de passe unique enregistré dans un gestionnaire ;
- l’authentification multifacteur ;
- une adresse de récupération pérenne ;
- des alertes de connexion et de renouvellement ;
- la limitation des comptes administrateurs ;
- la conservation du code ou mécanisme de récupération.

## 5.8 Transfert et réversibilité

La procédure de transfert, le code d’autorisation éventuel et les restrictions temporaires sont documentés. Avant un transfert, les zones DNS et paramètres utiles sont exportés ou relevés. Un transfert de registrar ne doit pas être confondu avec une modification d’hébergement ou de DNS.

## 5.9 Répartition des responsabilités

| Action | Claynum | Client | Registrar ou registre |
|---|---|---|---|
| Choix du nom | conseille et alerte | décide | — |
| Enregistrement | accompagne | souscrit, paie et reste titulaire | enregistre selon ses règles |
| Protection du compte | recommande et vérifie | conserve les facteurs et accès | fournit les mécanismes disponibles |
| Renouvellement | peut rappeler ou contrôler si prévu | reste responsable du paiement | applique le contrat |
| Transfert | prépare et accompagne | autorise | exécute la procédure |

> **POSITION CLAYNUM**  
> Pour le nom de domaine, Claynum accompagne. Le client en reste le titulaire, le payeur et le décideur.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Acteurs d’un nom de domaine  
> Objectif : distinguer titulaire, registrar, registre, gestionnaire DNS et hébergeur  
> Éléments : client titulaire, bureau d’enregistrement, Afnic ou autre registre, serveurs DNS, hébergeur  
> Type : schéma de rôles

# 6. Système de noms de domaine — DNS

## 6.1 Rôle du DNS

Le DNS est le système qui indique vers quel service diriger une demande portant sur un nom. Il relie par exemple claynum.fr à l’adresse du serveur qui héberge le site, et indique quels serveurs reçoivent les courriels du domaine.

Un même domaine contient plusieurs informations DNS. Elles sont stockées dans une zone gérée par des serveurs faisant autorité.

```text
claynum.fr     → 128.65.195.180      A
www.claynum.fr → claynum.fr          CNAME
claynum.fr     → serveur de messagerie MX
claynum.fr     → "v=spf1 ..."        TXT
```

## 6.2 Zone DNS et serveurs faisant autorité

Le registrar et le gestionnaire DNS peuvent être le même prestataire, mais leurs rôles diffèrent. Le registrar gère l’enregistrement du domaine ; le service DNS publie les enregistrements techniques. Les serveurs de noms déclarés pour le domaine doivent correspondre à l’endroit où la zone est réellement administrée.

Avant toute modification, Claynum identifie :

- le registrar ;
- les serveurs de noms actifs ;
- le gestionnaire de la zone ;
- les enregistrements existants ;
- les services qui en dépendent.

## 6.3 Enregistrements A et AAAA

Un enregistrement A associe un nom à une adresse IPv4. Un enregistrement AAAA l’associe à une adresse IPv6. Une modification erronée peut rendre le site ou un sous-domaine inaccessible.

Les adresses doivent provenir de l’hébergeur ou du service cible. Claynum ne devine pas une valeur et conserve l’état antérieur avant modification.

## 6.4 Alias CNAME

Un CNAME déclare qu’un nom est l’alias d’un autre nom. Il est couramment utilisé pour www, pour une plateforme d’hébergement ou pour un service tiers. Les contraintes du fournisseur cible doivent être respectées, notamment lorsque le domaine racine ne peut pas utiliser un CNAME classique.

## 6.5 Messagerie : MX, SPF, DKIM et DMARC

Les enregistrements MX désignent les serveurs qui reçoivent les messages. SPF, DKIM et DMARC contribuent à limiter l’usurpation du domaine et à améliorer la délivrabilité :

- SPF indique quels systèmes sont autorisés à émettre pour le domaine ;
- DKIM permet au serveur émetteur de signer les messages ;
- DMARC définit une politique de traitement et de rapport en s’appuyant sur l’alignement SPF ou DKIM.

Ces mécanismes doivent être cohérents avec tous les services d’envoi réellement utilisés. Une politique DMARC restrictive n’est mise en place qu’après inventaire et observation suffisante.

## 6.6 Enregistrements TXT de validation

De nombreux services demandent un enregistrement TXT pour vérifier la maîtrise d’un domaine. La valeur, sa durée de vie et la possibilité de la supprimer après validation sont documentées.

## 6.7 Sous-domaines

Les sous-domaines permettent de séparer des services : www, app, mail, espace-client ou test. Leur création doit rester lisible et éviter d’exposer inutilement des environnements internes.

## 6.8 Propagation et caches

Une modification DNS n’est pas nécessairement visible partout immédiatement. Les résolveurs conservent les réponses pendant la durée indiquée par le TTL. Avant une migration planifiée, le TTL peut être réduit suffisamment tôt, puis rétabli après stabilisation.

Le terme « propagation » simplifie un mécanisme de caches distribués : il ne signifie pas que la nouvelle information est activement poussée vers tous les serveurs d’Internet.

## 6.9 Modifications réalisées par Claynum

Pour le DNS, Claynum peut configurer lorsqu’un besoin précis est défini. Toute intervention suit la séquence suivante :

1. relever ou exporter la zone existante ;
2. identifier les services concernés ;
3. préparer la valeur et le retour arrière ;
4. obtenir la validation lorsque l’impact est significatif ;
5. appliquer la modification ;
6. contrôler la résolution et le service ;
7. consigner la date, l’auteur et la valeur finale.

## 6.10 Sauvegarde et traçabilité

L’état de la zone DNS est annexé à l’inventaire technique. Les enregistrements temporaires sont identifiés. Les comptes donnant accès à la zone suivent les règles de protection des comptes administrateurs.

> **POINT DE VIGILANCE**  
> Une zone DNS peut contenir des réglages dont l’utilité n’est pas immédiatement visible. La suppression d’un enregistrement ancien n’est jamais décidée sur sa seule apparence.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Du nom saisi dans le navigateur au serveur web  
> Objectif : expliquer simplement la résolution DNS et la distinction entre domaine, DNS et hébergement  
> Éléments : navigateur, résolveur DNS, serveurs faisant autorité, adresse IP, serveur d’hébergement  
> Type : flux technique simplifié

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Enregistrements DNS d’un domaine Claynum type  
> Objectif : montrer qu’un domaine porte plusieurs informations indépendantes  
> Éléments : A ou AAAA, CNAME, MX, SPF, DKIM, DMARC, TXT de validation  
> Type : carte annotée d’une zone DNS

# 7. Messagerie professionnelle

## 7.1 Choix du fournisseur

Le choix d’une messagerie professionnelle ne se limite pas au prix d’une boîte. Il prend en compte la fiabilité, la protection des comptes, les outils collaboratifs associés, la localisation et les conditions de traitement des données, les possibilités d’export, le support et les coûts de croissance.

Claynum distingue la messagerie fournie avec un hébergement web d’une suite collaborative complète. La première peut suffire pour quelques adresses et des usages simples ; la seconde apporte généralement une meilleure gestion des comptes, des calendriers, du partage et de la sécurité, au prix d’un abonnement récurrent.

## 7.2 Création des adresses et alias

Les adresses nominatives sont privilégiées pour les personnes ; les adresses fonctionnelles telles que contact@, facturation@ ou support@ sont créées comme boîtes, alias ou groupes selon le besoin réel.

Une adresse fonctionnelle ne doit pas dépendre durablement d’une personne. Les règles de transfert, de délégation et de départ d’un utilisateur sont documentées.

## 7.3 Configuration des terminaux

Claynum peut accompagner la configuration initiale sur un nombre défini de postes ou appareils. Cette configuration comprend les paramètres de connexion, la synchronisation, la signature et un test d’envoi et de réception.

Le support général des postes, téléphones, systèmes d’exploitation ou logiciels de messagerie n’est pas inclus sauf mention expresse.

## 7.4 Authentification multifacteur

L’authentification multifacteur est activée dès que le fournisseur le permet, en priorité pour les comptes administrateurs et les boîtes ayant accès à des informations sensibles. Les méthodes de récupération sont préparées sans créer un contournement plus faible que la protection principale.

Les utilisateurs sont informés que la double authentification ne protège pas contre toutes les attaques, notamment la validation imprudente d’une demande frauduleuse ou le détournement d’une session déjà ouverte.

## 7.5 Protection contre l’usurpation

La configuration DNS de messagerie est vérifiée : MX, SPF, DKIM et DMARC. La mise en place est progressive afin de ne pas bloquer des services d’envoi légitimes. Les rapports DMARC peuvent aider à identifier les sources d’émission, mais leur exploitation régulière constitue une prestation distincte.

## 7.6 Sauvegarde et conservation

La redondance du fournisseur ne constitue pas nécessairement une sauvegarde permettant de restaurer un message supprimé depuis longtemps. Les besoins de conservation, d’archivage et de restauration sont distingués.

Lorsque l’activité l’exige, une solution de sauvegarde ou d’archivage indépendante est étudiée. La durée de conservation répond à une finalité identifiée et non à la seule possibilité de conserver indéfiniment.

## 7.7 Continuité et récupération des accès

Le client conserve au moins :

- l’accès administrateur principal ;
- une méthode de récupération indépendante de la boîte concernée ;
- l’inventaire des comptes, alias et groupes ;
- les informations contractuelles du fournisseur ;
- une procédure de départ ou de remplacement d’un utilisateur.

## 7.8 Limites du support Claynum

Claynum peut intervenir sur la création, la configuration, la délivrabilité élémentaire et une migration limitée et cadrée. Ne sont pas inclus par défaut : l’assistance quotidienne aux utilisateurs, la restauration garantie de tout message, l’administration permanente d’une suite collaborative, la migration d’archives volumineuses ou la réponse à une compromission.

> **POSITION CLAYNUM**  
> La messagerie est un service critique. Le client doit en détenir l’administration et comprendre le coût récurrent, les mécanismes de récupération et les limites de conservation.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Parcours d’un courriel professionnel  
> Objectif : distinguer émission, contrôles DNS, transport, réception et consultation  
> Éléments : utilisateur, serveur émetteur, SPF-DKIM-DMARC, serveur destinataire, boîte et terminal  
> Type : flux simplifié

# 8. Hébergement et publication

## 8.1 Hébergement mutualisé, serveur privé et plateforme gérée

L’hébergement mutualisé fournit un environnement standard administré par le fournisseur. Il convient souvent aux sites vitrines et applications simples. Un serveur privé offre davantage de liberté mais transfère une part importante de l’administration, des mises à jour, de la surveillance et des sauvegardes au client ou à son prestataire.

Une plateforme gérée automatise le déploiement et certains services techniques. Elle peut réduire l’exploitation, mais crée une dépendance à son modèle, ses tarifs et ses limites.

## 8.2 Critères de choix

Le choix tient compte :

- des technologies supportées ;
- de la localisation des données ;
- du niveau d’administration requis ;
- des sauvegardes et restaurations disponibles ;
- des journaux accessibles ;
- des limites de trafic, stockage et exécution ;
- des certificats HTTPS ;
- des possibilités d’export et de migration ;
- du support et des engagements de service ;
- du coût à l’usage normal et en croissance.

## 8.3 Localisation des données

La localisation contractuelle et technique est vérifiée lorsque des données personnelles ou confidentielles sont hébergées. L’adresse commerciale d’un fournisseur ne suffit pas à déterminer le lieu de traitement ni les sous-traitants mobilisés.

Le niveau d’analyse est proportionné aux données. Un site purement public n’appelle pas les mêmes contrôles qu’une application contenant des fichiers clients.

## 8.4 Environnements de développement et de production

Les essais ne sont pas réalisés directement en production lorsqu’une erreur pourrait affecter le service ou les données. Selon la taille du projet, Claynum distingue :

- l’environnement local de développement ;
- un environnement de test ou de préproduction ;
- l’environnement de production.

Les données réelles ne sont pas copiées en test sans nécessité, protection et autorisation. Des jeux de données fictifs ou anonymisés sont privilégiés.

## 8.5 Certificats HTTPS

Tout service accessible sur Internet utilise HTTPS. Le certificat doit couvrir les noms réellement employés et être renouvelé automatiquement lorsque la plateforme le permet. Après configuration, Claynum vérifie la redirection depuis HTTP, la validité du certificat et l’absence de contenu chargé en clair.

HTTPS protège le transport ; il ne garantit ni la fiabilité du site ni l’identité commerciale de son éditeur au-delà des vérifications effectuées pour le certificat.

## 8.6 Déploiement et retour arrière

Le déploiement doit être reproductible. Pour une application, il précise au minimum la version publiée, les paramètres nécessaires, les migrations de données, les vérifications après mise en service et la possibilité de revenir à la version précédente.

Pour un site statique simple, une publication manuelle peut rester acceptable si elle est documentée et si une copie versionnée permet la restauration.

## 8.7 Journalisation et supervision élémentaire

Les journaux utiles à la compréhension d’une erreur sont activés sans enregistrer de mots de passe, jetons, données excessives ou contenus inutilement sensibles. Leur durée de conservation est limitée.

Une vérification de disponibilité ou une alerte élémentaire peut être mise en place. Elle ne constitue pas une supervision complète ni un engagement de rétablissement immédiat.

## 8.8 Sauvegardes

Les éléments à sauvegarder sont identifiés séparément : code, configuration, fichiers déposés, base de données et secrets nécessaires à la restauration. Une sauvegarde n’est utile que si elle est accessible, protégée et restaurable.

Le dispositif précise :

- la fréquence ;
- la durée de rétention ;
- le lieu de stockage ;
- le chiffrement éventuel ;
- le responsable du contrôle ;
- la fréquence des essais de restauration.

## 8.9 Renouvellements et dépendances contractuelles

Les services payants sont inventoriés avec leur titulaire, leur échéance, leur moyen de paiement et leur fonction. Un arrêt de paiement peut interrompre le site, la base de données, l’envoi de courriels ou le stockage.

## 8.10 Réversibilité

Avant de retenir un hébergement, Claynum vérifie qu’il est possible de récupérer les fichiers, le code, la configuration et les données dans un format exploitable. La procédure de sortie est testée ou décrite au niveau nécessaire.

> **POINT DE VIGILANCE**  
> La facilité de mise en ligne ne doit pas masquer l’exploitation. Un serveur privé non administré est rarement une économie ; il transforme un abonnement simple en responsabilité technique permanente.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Environnements et chaîne de publication  
> Objectif : montrer le passage du développement à la production avec validation et retour arrière  
> Éléments : poste de développement, dépôt de code, test, préproduction, production, sauvegarde  
> Type : pipeline de déploiement

# 9. Sites web

## 9.1 Site vitrine statique

Le site statique convient lorsque le contenu évolue peu et peut être mis à jour avec l’aide de Claynum. Il offre une surface technique réduite, de bonnes performances et une maintenance limitée. Il ne comporte pas d’interface d’administration ni de base de données par défaut.

Il constitue le choix de référence pour une présence en ligne simple : présentation de l’activité, services, zone géographique, réalisations, coordonnées et formulaire ou lien de contact.

## 9.2 Site administrable

Un système de gestion de contenu est retenu lorsque le client doit publier régulièrement et de manière autonome. Ce choix ajoute des comptes, des extensions, des mises à jour, une base de données et une surface d’attaque plus importante.

Avant de retenir cette option, Claynum vérifie que le besoin d’autonomie justifie la charge d’exploitation. Le nombre d’extensions est limité et leur maintenance est organisée.

## 9.3 Formulaires de contact

Un formulaire collecte uniquement les informations nécessaires au traitement de la demande. Il comporte une information sur l’usage des données et un moyen de contact alternatif.

Le traitement technique comprend :

- la validation des champs côté navigateur et côté serveur ;
- la protection contre les envois automatisés proportionnée au risque ;
- la limitation des pièces jointes ou leur exclusion ;
- la protection des destinataires contre l’exposition directe ;
- un message de confirmation qui ne révèle pas d’information sensible ;
- une durée de conservation cohérente.

## 9.4 Référencement naturel élémentaire

Le référencement élémentaire repose sur un contenu compréhensible, des titres structurés, une adresse stable, des métadonnées cohérentes, un site mobile et rapide, ainsi qu’une indexation techniquement possible.

Claynum ne garantit pas une position dans les moteurs de recherche. Le référencement concurrentiel, l’achat de mots-clés, la production éditoriale continue et l’analyse avancée relèvent d’une prestation spécialisée.

## 9.5 Mesure d’audience

La mesure d’audience doit répondre à une question : nombre de visites, origine générale, pages consultées ou conversion d’un formulaire. L’outil le plus simple couvrant le besoin est privilégié.

La présence de traceurs, leur finalité et les conditions d’exemption ou de consentement sont vérifiées. La CNIL rappelle que certains traceurs nécessitent une information et un consentement préalables, tandis que d’autres peuvent être exemptés sous conditions. Une bannière de consentement n’est donc ni systématiquement nécessaire ni suffisante à elle seule.

## 9.6 Accessibilité et compatibilité mobile

Le site est conçu pour rester lisible au clavier, sur écran étroit et avec un zoom important. Les titres, libellés, contrastes, messages d’erreur et textes alternatifs sont vérifiés selon le niveau convenu.

Claynum vise de bonnes pratiques d’accessibilité. Une déclaration de conformité ou un audit réglementaire complet n’est produit que dans le cadre d’une mission spécifique avec méthode et compétence adaptées.

## 9.7 Performance

Les images sont dimensionnées et compressées, les ressources inutiles supprimées et le chargement des scripts limité. La performance est contrôlée dans des conditions réalistes, notamment sur mobile.

Les objectifs doivent rester cohérents avec les fonctions et services tiers. Une vidéo, une carte interactive ou un outil de mesure d’audience peut dégrader le temps de chargement.

## 9.8 Mentions légales, cookies et données personnelles

Tout site professionnel doit permettre d’identifier son éditeur et son hébergeur selon le statut applicable. Les informations relatives aux données personnelles et aux traceurs doivent être accessibles et cohérentes avec le fonctionnement réel du site.

Claynum prépare les emplacements, inventorie les traitements techniques et peut intégrer les textes fournis ou validés par le client. Claynum ne rédige pas seul un avis juridique définitif. Les sources officielles Entreprendre.Service-Public.fr et CNIL sont vérifiées avant publication.

## 9.9 Publication et recette

La recette d’un site vérifie au minimum :

- les contenus et coordonnées ;
- les liens et boutons ;
- le formulaire et la réception des messages ;
- l’affichage mobile et les principaux navigateurs ;
- HTTPS et les redirections ;
- les métadonnées et l’indexation ;
- les mentions et informations sur les données ;
- l’absence de contenu de test ;
- la sauvegarde de la version publiée.

## 9.10 Maintenance et évolution

Pour un site statique, la maintenance peut se limiter aux changements de contenu, au contrôle périodique des liens et à l’environnement d’hébergement. Pour un site administrable, elle comprend en plus les mises à jour, les sauvegardes, la compatibilité des extensions et le contrôle des comptes.

> **POSITION CLAYNUM**  
> Le site vitrine statique est la solution de référence lorsque le client n’a pas un besoin réel de publication autonome. Il réduit les coûts, les dépendances et la surface d’attaque.

# 10. Applications sur mesure

## 10.1 Critères justifiant une application spécifique

Une application sur mesure est pertinente lorsqu’un besoin métier ne peut pas être couvert convenablement par un outil existant raisonnable, ou lorsque l’adaptation d’un produit serait plus coûteuse et contraignante que la réalisation ciblée.

Avant de développer, Claynum examine :

- les outils déjà utilisés ;
- la possibilité de simplifier le processus ;
- les produits standards disponibles ;
- les besoins réellement différenciants ;
- la durée de vie attendue ;
- le coût de maintenance ;
- la capacité du client à participer à la recette.

## 10.2 Applications web

L’application web est accessible au moyen d’un navigateur. Elle facilite l’usage sur plusieurs appareils et le déploiement centralisé. Elle nécessite cependant un hébergement, une gestion des accès, une protection des échanges et une exploitation proportionnée aux données et à la criticité.

Pour une petite application, une architecture monolithique claire est souvent préférable à une multiplication de services. Les composants sont séparés lorsque cette séparation répond à un besoin concret de sécurité, de charge ou d’évolution.

## 10.3 Applications de bureau

Une application de bureau peut convenir à un usage individuel ou local, notamment lorsqu’un fonctionnement hors ligne, l’accès à des fichiers locaux ou une interface dédiée est utile.

Le périmètre précise les systèmes supportés, le mode d’installation, les mises à jour, le stockage local, les sauvegardes et l’export des données. La distribution à grande échelle ou la signature de logiciels peut nécessiter une prestation supplémentaire.

## 10.4 Applications mobiles

Claynum peut réaliser un prototype, une application web installable ou un paquet de test Android. La publication sur les magasins Apple ou Google n’est pas incluse par défaut : elle implique comptes développeur, règles de publication, signatures, politiques de confidentialité, suivi des versions et contraintes propres aux plateformes.

Une application mobile native n’est retenue que si les fonctions du terminal, le mode hors ligne ou l’expérience attendue le justifient.

## 10.5 Maquettes et prototypes

La maquette valide l’organisation des écrans et le vocabulaire. Le prototype valide une interaction ou une hypothèse technique. Aucun des deux ne doit être présenté comme une application prête pour la production sans vérification explicite.

Les éléments qui ne sont pas fonctionnels sont identifiés. Les données de démonstration ne sont pas confondues avec des données réelles.

## 10.6 Architecture fonctionnelle et technique

L’architecture décrit au niveau utile :

- les utilisateurs et leurs rôles ;
- les fonctions principales ;
- les composants ;
- les flux de données ;
- les services externes ;
- le stockage ;
- les mécanismes d’authentification ;
- les sauvegardes ;
- le déploiement.

La documentation doit permettre à un tiers compétent de comprendre la solution sans transformer un petit projet en dossier d’architecture disproportionné.

## 10.7 Authentification et gestion des droits

Chaque utilisateur dispose d’un compte nominatif lorsqu’une traçabilité ou une personnalisation est nécessaire. Les rôles sont définis à partir des actions métier et non de titres vagues. Les contrôles sont appliqués côté serveur ; masquer un bouton dans l’interface ne suffit pas à interdire l’action.

Pour les besoins simples, le nombre de rôles est limité. Les comptes administrateurs sont séparés des usages ordinaires lorsque le risque le justifie.

## 10.8 Interfaces avec des services tiers

Une API ou un service externe ajoute une dépendance : disponibilité, authentification, quotas, tarification, évolution et traitement des données. Le contrat indique ce qui se passe si le service change ou devient indisponible.

Les clés d’API sont stockées comme secrets et non dans le code ou le navigateur lorsqu’elles permettent une action privilégiée.

## 10.9 Tests et recette

Les tests portent en priorité sur :

- les parcours essentiels ;
- les règles métier ;
- les droits d’accès ;
- les erreurs et entrées invalides ;
- les imports et exports ;
- les sauvegardes et restaurations ;
- les interfaces externes ;
- les conditions de déploiement.

La recette est réalisée à partir de cas convenus, avec des exemples valides et invalides. Les anomalies sont classées selon leur effet sur l’usage et la mise en service.

## 10.10 Documentation et code source

Le dossier de remise précise :

- l’adresse du dépôt ou l’archive du code ;
- la version livrée ;
- les instructions d’installation et de déploiement ;
- les paramètres nécessaires ;
- les dépendances et licences significatives ;
- la structure des données ;
- les comptes et services externes ;
- les limites connues.

La propriété intellectuelle et les droits de réutilisation sont définis contractuellement. Les composants tiers restent soumis à leurs licences.

## 10.11 Hébergement, exploitation et maintenance

Une application livrée a besoin d’un responsable d’exploitation, même si la charge est faible. Le contrat désigne qui surveille les échéances, applique les mises à jour, contrôle les sauvegardes et traite les alertes.

Sans contrat de maintenance, Claynum remet la solution et intervient uniquement sur demande acceptée.

## 10.12 Conditions d’évolution

Une évolution est distinguée d’une correction. Une correction rétablit le comportement décrit et accepté. Une évolution modifie le besoin, ajoute une fonction ou adapte la solution à une nouvelle contrainte externe.

> **POINT DE VIGILANCE**  
> Une application qui fonctionne en démonstration n’est pas automatiquement prête pour la production. Les données, les droits, les sauvegardes, le déploiement et l’exploitation font partie du produit réel.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Architecture type d’une application web Claynum  
> Objectif : montrer les composants sans imposer une technologie particulière  
> Éléments : navigateur, application, authentification, base de données, stockage, service externe, sauvegarde  
> Type : architecture logique

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : De la maquette à la mise en service  
> Objectif : distinguer maquette, prototype, version de test, recette et production  
> Éléments : besoin, maquette, prototype, développement, tests, recette, déploiement  
> Type : cycle itératif

# 11. Données et bases de données

## 11.1 Qualification des données

Avant toute conception, Claynum identifie les catégories de données, leur origine, leur propriétaire métier, leur sensibilité, leur durée de vie et les utilisateurs autorisés. Une donnée disponible n’est pas nécessairement utile ni licite à collecter.

Les données temporaires, calculées, importées et de référence sont distinguées afin de définir les sauvegardes et les règles de suppression.

## 11.2 Modélisation et stockage

Le modèle de données traduit les objets métier et leurs relations. Il évite les champs polyvalents dont le sens change selon le contexte, les duplications incontrôlées et les valeurs non vérifiables.

Le choix entre fichier structuré, base relationnelle, stockage documentaire ou service géré dépend du besoin. Une base de données n’est pas retenue lorsque quelques fichiers versionnés suffisent ; elle devient nécessaire lorsque plusieurs utilisateurs modifient des informations reliées et qu’une cohérence doit être garantie.

## 11.3 Import et export

Tout import comprend :

- un format attendu ;
- des exemples valides et invalides ;
- une validation avant écriture ;
- un rapport des lignes rejetées ;
- une stratégie en cas d’import partiel ;
- une sauvegarde avant opération importante.

L’export utilise un format ouvert ou largement exploitable lorsque cela est possible. Les encodages, séparateurs, dates et identifiants sont documentés.

## 11.4 Contrôles de cohérence

Les contrôles sont placés au bon niveau : interface pour guider l’utilisateur, serveur pour garantir la règle, base de données pour protéger les contraintes fondamentales. Les listes de valeurs, formats, unicités et relations obligatoires sont explicites.

Une expression régulière peut vérifier une forme précise, mais elle ne valide pas à elle seule le sens ou l’existence d’une donnée.

## 11.5 Sauvegarde et restauration

Une sauvegarde de base de données doit être cohérente avec les fichiers qui lui sont liés. La procédure décrit l’outil, la fréquence, le chiffrement, la rétention, le stockage et la restauration.

Un essai de restauration est réalisé avant la mise en service ou selon une fréquence proportionnée. Le résultat et le temps nécessaire sont consignés.

## 11.6 Durées de conservation

La durée de conservation est définie par finalité, obligation ou besoin démontré. Elle inclut les archives et sauvegardes, avec des modalités adaptées lorsqu’une suppression immédiate dans chaque sauvegarde n’est pas techniquement possible.

## 11.7 Accès administratifs

Les accès directs à la base sont limités. Les opérations courantes passent par l’application. Les comptes d’administration sont nominatifs ou attribuables, protégés et utilisés uniquement lorsque nécessaire.

Les exports contenant des données personnelles ou confidentielles sont protégés et supprimés après usage.

## 11.8 Portabilité et restitution

Le client doit pouvoir récupérer ses données dans un format défini. La restitution précise les données incluses, le format, les relations, les pièces jointes, l’encodage et la date d’extraction.

## 11.9 Suppression en fin de prestation

Après validation de la remise, Claynum supprime les copies de travail qui ne sont plus nécessaires, sous réserve des obligations de conservation et de la preuve contractuelle utile. Les accès sont révoqués et la suppression est consignée lorsque l’enjeu le justifie.

> **POSITION CLAYNUM**  
> Les données appartiennent au fonctionnement du client. Leur export, leur compréhension et leur restitution ne doivent pas dépendre d’un mécanisme opaque maîtrisé uniquement par Claynum.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Cycle de vie d’une donnée  
> Objectif : relier collecte, usage, sauvegarde, archivage, restitution et suppression  
> Éléments : collecte, validation, stockage, consultation, export, sauvegarde, archive, suppression  
> Type : cycle de vie

# 12. Sécurité minimale applicable

## 12.1 Approche proportionnée au risque

La sécurité n’est pas un module ajouté en fin de projet. Elle commence par la réduction du périmètre, des données et des comptes. Claynum applique un socle minimal à toute solution et renforce les mesures selon la sensibilité, l’exposition et les conséquences d’un incident.

Le guide de sécurité des données personnelles de la CNIL et les ressources de l’ANSSI constituent des références. Leur application complète peut dépasser le périmètre d’une petite prestation ; les écarts significatifs sont alors signalés et orientés vers un spécialiste.

## 12.2 Gestion des comptes

Chaque compte correspond à une personne ou une fonction identifiée. Les comptes inutilisés sont désactivés. Les comptes administrateurs sont limités et séparés des usages ordinaires lorsque possible.

Les droits sont accordés selon le besoin réel, revus lors d’un changement de rôle et retirés au départ d’un utilisateur.

## 12.3 Mots de passe et authentification multifacteur

Les mots de passe sont uniques, suffisamment longs et conservés dans un gestionnaire adapté. Claynum ne stocke pas les mots de passe des utilisateurs en clair. Une application qui gère elle-même des mots de passe utilise un mécanisme de hachage éprouvé fourni par le cadre technique retenu.

L’authentification multifacteur est activée en priorité sur les comptes d’administration, les fournisseurs cloud, la messagerie, le registrar et les dépôts de code.

## 12.4 Secrets et clés d’accès

Les mots de passe techniques, clés d’API, jetons et certificats privés sont séparés du code. Ils ne sont pas envoyés dans un courriel non protégé ni placés dans un document partagé sans contrôle.

Un secret exposé est remplacé ; le supprimer de la dernière version du code ne suffit pas s’il demeure dans l’historique ou a déjà été copié.

## 12.5 Principe du moindre privilège

Chaque utilisateur, composant et service reçoit uniquement les droits nécessaires. Une application ne se connecte pas à la base avec un compte d’administration générale si elle n’en a pas besoin. Les environnements de test n’utilisent pas les secrets de production.

## 12.6 Mises à jour et dépendances

Les systèmes, cadres de développement et bibliothèques sont suivis. Les versions non maintenues sont évitées. Une mise à jour importante est testée avant production et accompagnée d’une possibilité de retour arrière.

Les alertes automatiques de dépendances sont utiles mais ne remplacent pas l’analyse de l’exposition réelle et de l’impact d’une mise à jour.

## 12.7 Chiffrement des échanges et des supports

Les échanges sur Internet utilisent TLS. Le chiffrement au repos est envisagé selon les données, l’hébergement et le risque de perte du support. Les sauvegardes contenant des données sensibles sont protégées au même niveau que la production.

La gestion des clés est prise en compte : un chiffrement dont la clé est perdue rend les données irrécupérables ; une clé stockée avec les données offre une protection limitée.

## 12.8 Sauvegardes et restauration

Le dispositif de sauvegarde vise à résister à une erreur, une panne et, si l’enjeu le justifie, une compromission. Une copie indépendante ou non modifiable par le compte courant est privilégiée. La règle dite « 3-2-1 » peut servir de repère, mais le dispositif réel est adapté au contexte.

La restauration est testée. Le client connaît la perte de données maximale et le délai de reprise visés, sans confondre ces objectifs avec une garantie contractuelle non souscrite.

## 12.9 Journalisation

Les événements utiles sont enregistrés : erreurs, connexions, modifications administratives et opérations sensibles selon le besoin. Les journaux sont protégés, horodatés, limités dans le temps et consultés dans le respect de leur finalité.

Les mots de passe, jetons complets et données excessives ne doivent pas apparaître dans les journaux. La CNIL rappelle que les traces ne doivent pas être réutilisées pour une finalité étrangère à la sécurité et au bon fonctionnement du système.

## 12.10 Vulnérabilités et incidents

Lorsqu’une vulnérabilité ou un incident est signalé, Claynum :

1. qualifie les faits sans effacer les traces utiles ;
2. limite l’exposition si une action sûre est possible ;
3. informe le client et identifie le responsable de décision ;
4. recommande le recours à un prestataire spécialisé si nécessaire ;
5. documente les actions réalisées ;
6. participe à la restauration dans le périmètre accepté.

La notification d’une violation de données, les relations avec les autorités et l’investigation approfondie relèvent du responsable de traitement et, selon le cas, de professionnels spécialisés.

## 12.11 Limites de Claynum en cybersécurité

Claynum met en œuvre de bonnes pratiques et signale les risques visibles. Cette prestation ne vaut pas audit de sécurité, homologation, certification, test d’intrusion, surveillance SOC ou garantie d’absence de vulnérabilité.

> **POINT DE VIGILANCE**  
> La sécurité déclarative est insuffisante. Une mesure n’est considérée comme en place que si elle est configurée, vérifiée et attribuée à un responsable pour la durée de vie du service.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Défense en profondeur d’un service Claynum  
> Objectif : montrer la complémentarité des mesures sans promettre une sécurité absolue  
> Éléments : identité, droits, application, données, sauvegardes, journaux, mises à jour  
> Type : couches concentriques ou empilées

# 13. Données personnelles et conformité

## 13.1 Identifier les traitements

Un traitement de données personnelles existe dès lors qu’une information se rapporte directement ou indirectement à une personne identifiable. Un formulaire de contact, un fichier clients, une liste d’adhérents, des journaux de connexion ou une mesure d’audience peuvent être concernés.

Pour chaque traitement lié à la solution, la fiche de cadrage précise :

- la finalité ;
- les personnes concernées ;
- les catégories de données ;
- les destinataires ;
- la durée de conservation ;
- les fournisseurs impliqués ;
- les mesures de sécurité ;
- le moyen d’exercer les droits.

## 13.2 Données strictement nécessaires

La collecte est limitée à ce qui sert effectivement la finalité. Un champ est supprimé s’il n’est pas utilisé ou si son intérêt ne justifie pas le risque et la charge de gestion.

Les champs libres sont encadrés lorsqu’ils pourraient conduire les utilisateurs à saisir des informations sensibles non prévues. Les pièces jointes sont évitées dans un simple formulaire de contact.

## 13.3 Information des personnes

L’information doit être compréhensible, accessible au moment de la collecte et cohérente avec la pratique réelle. Elle indique notamment l’identité du responsable de traitement, la finalité, la base juridique retenue, les destinataires, la durée ou ses critères, les droits et le point de contact.

Claynum peut intégrer une mention fournie ou validée par le client et signaler les informations manquantes. Le choix de la base juridique et la validation du texte relèvent du responsable de traitement et, lorsque nécessaire, de son conseil.

## 13.4 Consentement et cookies

Le consentement n’est pas la base de toutes les opérations. Il doit être utilisé lorsqu’il est pertinent et répondre aux conditions applicables. Pour les cookies et autres traceurs, la CNIL distingue ceux qui nécessitent un consentement préalable de ceux qui peuvent en être exemptés sous conditions.

Avant d’installer une bannière, Claynum inventorie les traceurs, leurs fournisseurs, leurs finalités et leur durée. Aucun traceur soumis au consentement ne doit être déposé avant un choix valide. Refuser doit être aussi accessible qu’accepter lorsque le consentement est requis.

## 13.5 Sous-traitants techniques

Le fournisseur d’hébergement, de messagerie, d’analyse ou d’envoi peut traiter des données pour le compte du client. Son rôle, ses garanties, ses sous-traitants ultérieurs et les transferts éventuels sont examinés.

Lorsque Claynum traite des données personnelles pour le compte du client, les obligations correspondantes sont encadrées par écrit. L’article 28 du RGPD prévoit notamment que le contrat définisse l’objet, la durée, la nature, la finalité, les catégories de données et de personnes, ainsi que les droits et obligations des parties.

## 13.6 Conservation et suppression

Les durées sont définies avant la mise en service. Les mécanismes de suppression peuvent être manuels pour un petit volume, à condition d’être attribués et réellement exécutés. Une automatisation est préférable lorsque la fréquence ou le volume rend le contrôle manuel incertain.

Les sauvegardes suivent un cycle de rétention distinct. La remise en production d’une ancienne sauvegarde doit être accompagnée des suppressions ou corrections intervenues depuis, lorsque cela est nécessaire.

## 13.7 Exercice des droits

La solution doit permettre de rechercher, corriger, exporter ou supprimer une personne sans opération disproportionnée. Le client définit le canal de réception des demandes et la personne chargée d’y répondre.

Claynum peut fournir une extraction technique ou une fonction adaptée. Claynum ne décide pas si une demande doit être acceptée ou refusée.

## 13.8 Rôle de Claynum et responsabilité du client

Dans la plupart des projets, le client détermine la finalité et les moyens essentiels : il est responsable de traitement. Claynum peut être sous-traitant lorsqu’il développe, maintient ou héberge techniquement pour son compte, ou intervenir comme simple fournisseur sans accès aux données selon le cas.

La qualification dépend des faits et non du seul intitulé du contrat. Elle est clarifiée avant tout accès à des données réelles.

## 13.9 Recours à un conseil juridique ou à un DPO

Un avis spécialisé est recommandé notamment lorsque le projet implique :

- des données sensibles ou des personnes vulnérables ;
- une surveillance régulière ;
- une décision automatisée significative ;
- un transfert complexe hors de l’Espace économique européen ;
- une collecte à grande échelle ;
- une obligation sectorielle ;
- une analyse d’impact ;
- un désaccord sur les rôles.

> **POINT DE VIGILANCE**  
> Une page « Politique de confidentialité » ne suffit pas à rendre un traitement conforme. Le texte, les réglages, les contrats, les durées et les pratiques doivent décrire la même réalité.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Rôles autour des données personnelles  
> Objectif : distinguer personne concernée, responsable de traitement, Claynum et fournisseurs techniques  
> Éléments : utilisateur, client, Claynum, hébergeur, outil de mesure, destinataires  
> Type : schéma de responsabilités

# 14. Déroulement d’une prestation

## 14.1 Premier échange

Le premier échange vise à comprendre le contexte, l’objectif, l’urgence et l’ordre de grandeur. Il ne constitue pas encore une étude complète. Claynum reformule la demande et indique les informations nécessaires à la qualification.

## 14.2 Diagnostic

Le diagnostic décrit l’existant, les difficultés, les utilisateurs, les données, les contraintes et les risques. Il peut conclure qu’une amélioration de l’organisation ou d’un outil existant est préférable à un développement.

## 14.3 Reformulation du besoin

La reformulation exprime le résultat attendu en langage métier, les utilisateurs concernés et les critères de réussite. Elle distingue les besoins indispensables, utiles et différables.

Une formulation type est : « permettre à [utilisateur] de [action] afin de [résultat], avec [contrainte essentielle] ».

## 14.4 Proposition de solution

La proposition présente :

- la solution recommandée ;
- les options écartées ou alternatives utiles ;
- les hypothèses ;
- les livrables ;
- les responsabilités ;
- les services tiers et coûts récurrents ;
- les limites ;
- le planning indicatif ;
- les conditions de recette et de maintenance.

## 14.5 Définition du périmètre

Le périmètre décrit ce qui est inclus et ce qui ne l’est pas. Les mots « simple », « intuitif », « sécurisé » ou « complet » sont remplacés par des critères vérifiables.

Les changements demandés après validation sont analysés comme correction, précision ou évolution. Leur effet sur le coût et le délai est expliqué avant réalisation.

## 14.6 Maquette ou prototype

Une maquette est proposée lorsque l’interface ou l’organisation de l’information constitue un risque d’incompréhension. Un prototype est utilisé lorsqu’une faisabilité technique, une interaction ou un import doit être validé.

Le client valide le principe avant que Claynum n’investisse dans les détails de production.

## 14.7 Réalisation par itérations

Chaque itération produit un résultat visible, testé au niveau utile et présenté au client. Les retours sont regroupés, arbitrés et tracés. Les détails cosmétiques ne retardent pas la validation d’une fonction fondamentale.

Le rythme dépend de la taille du projet. Pour une petite application, quelques jalons simples suffisent : structure, parcours principal, données, finition, recette.

## 14.8 Recette et validation

La recette utilise des scénarios convenus et des données représentatives. Une anomalie bloquante empêche l’usage essentiel ; une anomalie majeure dégrade fortement une fonction ; une anomalie mineure n’empêche pas l’usage et peut être corrigée après mise en service selon l’accord.

La validation est formalisée par un procès-verbal, un courriel explicite ou le mécanisme prévu au contrat.

## 14.9 Mise en service

La mise en service est préparée par une liste de contrôle : sauvegarde, version, paramètres, comptes, DNS, HTTPS, données, tests, communication et retour arrière. Une plage adaptée est choisie lorsque l’opération peut interrompre un service existant.

## 14.10 Formation et remise documentaire

Les utilisateurs ou administrateurs désignés reçoivent les explications nécessaires. La remise comprend les accès, l’inventaire, les procédures et les limites connues. Les secrets ne sont pas placés dans le même document que leur contexte d’usage lorsque cela crée un risque inutile.

## 14.11 Clôture et bilan

La clôture vérifie :

- la validation des livrables ;
- la remise des accès et données ;
- la révocation des accès temporaires ;
- les services et coûts récurrents ;
- le sort des copies de travail ;
- la garantie ou maintenance applicable ;
- les améliorations éventuellement reportées.

> **POSITION CLAYNUM**  
> Le client est associé tôt et régulièrement. La recette ne doit pas être la première fois qu’il voit le fonctionnement réel de la solution.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Cycle complet d’une prestation Claynum  
> Objectif : donner une vue d’ensemble utilisable avec le client  
> Éléments : échange, diagnostic, cadrage, proposition, maquette, réalisation, recette, mise en service, remise  
> Type : cycle en étapes avec boucles d’itération

# 15. Exploitation, maintenance et assistance

## 15.1 Garantie de correction initiale

Le contrat peut prévoir une période pendant laquelle Claynum corrige sans coût supplémentaire les anomalies reproductibles qui empêchent le livrable de respecter le périmètre validé. Cette garantie ne couvre pas une évolution du besoin, une mauvaise utilisation, une modification par un tiers ou un changement de service externe.

La durée, le point de départ et le canal de signalement sont indiqués.

## 15.2 Maintenance corrective

La maintenance corrective vise à rétablir le comportement prévu. Le signalement comprend les étapes, le résultat attendu, le résultat observé, la date, l’environnement et, si possible, une capture dépourvue de données sensibles.

Claynum qualifie l’origine avant de s’engager sur une correction : code livré, hébergement, navigateur, fournisseur tiers, donnée invalide ou changement externe.

## 15.3 Maintenance évolutive

La maintenance évolutive ajoute ou modifie une fonction. Elle fait l’objet d’un cadrage et d’une estimation. Une accumulation de petites modifications peut justifier une nouvelle version et une recette regroupée.

## 15.4 Mises à jour techniques

Les mises à jour sont classées selon leur urgence, leur exposition et leur risque de régression. Une mise à jour de sécurité critique peut nécessiter une intervention rapide ; une montée de version majeure doit être préparée et testée.

Le contrat précise si la veille et l’application des mises à jour sont assurées par Claynum, par l’hébergeur ou par le client.

## 15.5 Assistance utilisateur

L’assistance porte uniquement sur les fonctions et utilisateurs définis. Elle ne remplace pas une formation générale au poste de travail, au système d’exploitation ou à un service tiers.

Les demandes sont centralisées par un interlocuteur lorsque le nombre d’utilisateurs le justifie. Cette organisation évite les demandes contradictoires et permet de distinguer incident, question et évolution.

## 15.6 Délais d’intervention

Sans engagement contractuel, les délais sont indicatifs et dépendent de la disponibilité. Un délai garanti nécessite un périmètre, des horaires, un canal, un niveau de priorité et une contrepartie adaptés.

Claynum ne promet pas un rétablissement qu’il ne maîtrise pas, notamment lorsque l’incident dépend d’un fournisseur tiers.

## 15.7 Absence d’astreinte

Claynum n’assure pas d’astreinte ni de présence permanente par défaut. Les services nécessitant une intervention 24 h/24 ou un délai de reprise très court sont orientés vers un opérateur disposant de l’organisation nécessaire.

## 15.8 Fin de maintenance et réversibilité

La fin de maintenance prévoit :

- la date de fin ;
- l’état des versions ;
- les demandes en cours ;
- la remise des accès et documents actualisés ;
- l’export des données ;
- le transfert vers un nouveau prestataire ;
- la révocation des accès Claynum ;
- la suppression des copies non nécessaires.

| Situation | Inclus dans une correction | À cadrer comme évolution | Hors périmètre par défaut |
|---|---|---|---|
| Fonction conforme au contrat mais jugée désormais insuffisante | — | oui | — |
| Erreur reproductible dans le code livré | oui | — | — |
| Nouvelle règle métier | — | oui | — |
| Panne générale de l’hébergeur | diagnostic éventuel | — | rétablissement du fournisseur |
| Compromission nécessitant investigation | mesures conservatoires limitées | — | réponse à incident spécialisée |

> **POINT DE VIGILANCE**  
> La maintenance ne doit pas devenir une obligation indéfinie née d’échanges informels. Son contenu, sa durée et ses délais sont écrits.

# 16. Propriété, accès et réversibilité

## 16.1 Titularité des comptes fournisseurs

Les comptes structurants sont créés au nom du client. Claynum utilise un accès délégué ou nominatif. Lorsque le fournisseur ne permet pas la délégation, l’usage d’un compte partagé reste exceptionnel, limité et suivi d’un changement de mot de passe.

## 16.2 Propriété du nom de domaine

Le client est titulaire du domaine, y compris lorsque Claynum a conseillé le choix et guidé l’enregistrement. Les coordonnées de récupération ne dépendent pas d’une adresse contrôlée uniquement par Claynum.

## 16.3 Contenus et données

Le client fournit ou valide les textes, images, logos et données. Il garantit disposer des droits nécessaires. Claynum signale les éléments manifestement problématiques mais ne réalise pas une recherche exhaustive de droits sans mission spécifique.

Les données du client lui sont restituées selon le format prévu. Claynum ne les réutilise pas pour un autre projet sans autorisation et base appropriée.

## 16.4 Code source et composants tiers

Le contrat précise les droits accordés sur les développements spécifiques : utilisation, modification, remise à un tiers et réutilisation éventuelle de composants génériques. Les bibliothèques, polices, images, modèles et services tiers conservent leurs propres licences.

Le dépôt remis ne contient pas de secret actif. Les éléments nécessaires sont fournis séparément ou recréés dans l’environnement du client.

## 16.5 Licences logicielles

Les licences significatives sont inventoriées. Une dépendance gratuite n’est pas nécessairement libre de toute obligation. Les licences incompatibles avec l’usage ou la redistribution prévus sont évitées.

## 16.6 Remise des identifiants

La remise des accès est effectuée par un canal adapté. Le client confirme la récupération puis modifie, lorsque nécessaire, les secrets temporaires. Les codes de secours multifacteur sont placés sous son contrôle.

Claynum conserve uniquement les accès nécessaires à une maintenance active et acceptée.

## 16.7 Export des données

L’export de réversibilité comprend les données utiles, leur structure, les fichiers liés et les informations nécessaires à l’interprétation. Une archive illisible sans l’application ne constitue pas une restitution suffisante si un format ouvert était raisonnablement possible.

## 16.8 Fin de prestation

La fin de prestation est considérée comme effective lorsque les livrables sont validés, les accès remis, les dépendances connues et les responsabilités futures explicites. Une fiche de clôture évite de laisser des comptes, abonnements ou sauvegardes sans responsable.

> **POSITION CLAYNUM**  
> La réversibilité est préparée dès le choix de la solution. Elle ne se résume pas à transmettre une archive au moment où la relation se termine.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Réversibilité d’une solution Claynum  
> Objectif : montrer ce qui doit pouvoir être transféré à un client ou à un nouveau prestataire  
> Éléments : domaine, comptes, code, configuration, données, documentation, sauvegardes, contrats  
> Type : paquet de remise avec destinations

# 17. Matrice des responsabilités

## 17.1 Principes de lecture

La matrice clarifie quatre positions :

- Réaliser : Claynum exécute l’action prévue ;
- Accompagner : Claynum guide, prépare ou contrôle, mais le client agit ou valide ;
- Conseiller : Claynum présente les options et conséquences ;
- Exclure ou orienter : l’action nécessite un autre intervenant ou un contrat distinct.

Ces positions peuvent évoluer pour une prestation particulière, mais toute dérogation est écrite.

## 17.2 Matrice générale « réalisé, accompagné, conseillé ou exclu »

| Domaine | Position standard Claynum | Responsabilité principale du client | Limite ou tiers concerné |
|---|---|---|---|
| Choix du domaine | conseiller et accompagner | décider et vérifier l’usage commercial | conseil en propriété industrielle si risque |
| Enregistrement du domaine | accompagner | souscrire, payer, rester titulaire | registrar et registre |
| Configuration DNS | réaliser sur demande cadrée | valider les services et conserver les accès | opérateur DNS pour disponibilité |
| Messagerie | conseiller, configurer et accompagner | administrer les utilisateurs et usages | fournisseur de messagerie |
| Hébergement | conseiller et déployer selon projet | souscrire et payer | hébergeur responsable de sa plateforme |
| Site vitrine | réaliser | fournir et valider les contenus | conseil juridique pour textes sensibles |
| Application sur mesure | réaliser dans le périmètre accepté | définir les règles métier et recetter | partenaire pour haute criticité |
| Base de données | concevoir et mettre en œuvre | définir les données et durées | spécialiste pour données réglementées |
| Sauvegardes | configurer si inclus | décider des objectifs et contrôler selon contrat | fournisseur de stockage |
| Sécurité de base | intégrer et vérifier | gérer utilisateurs et décisions | auditeur ou prestataire cyber spécialisé |
| RGPD | aider à inventorier et traduire techniquement | assumer le rôle de responsable de traitement | DPO ou juriste |
| Maintenance | réaliser si contrat | signaler et arbitrer | fournisseurs tiers selon l’incident |
| Astreinte 24 h/24 | exclure | choisir un opérateur adapté | prestataire d’exploitation |

## 17.3 RACI simplifié d’une prestation type

La notation suivante peut être utilisée : R = réalise, A = approuve et répond du résultat, C = consulté, I = informé.

| Activité | Claynum | Client | Fournisseur tiers | Spécialiste éventuel |
|---|---|---|---|---|
| Définition du besoin | R | A | I | C |
| Choix de la solution | R | A | C | C |
| Souscription des services | C | A/R | R pour l’activation | I |
| Réalisation technique | A/R | C | C | R sur son lot |
| Validation métier | C | A/R | I | C |
| Mise en service | R | A | C | C |
| Exploitation après remise | selon contrat | A | R sur sa plateforme | selon contrat |
| Conformité métier et juridique | C | A/R | C | R en conseil spécialisé |

## 17.4 Responsabilités du client

Le client :

- désigne un interlocuteur et prend les décisions ;
- fournit des informations et contenus exacts ;
- dispose des droits sur les éléments transmis ;
- valide les règles métier et les résultats ;
- reste titulaire de ses contrats et comptes ;
- gère les utilisateurs après remise sauf contrat contraire ;
- respecte les obligations propres à son activité ;
- signale les incidents et changements utiles.

## 17.5 Responsabilités de Claynum

Claynum :

- reformule le besoin et alerte sur les incohérences visibles ;
- réalise les livrables convenus avec diligence ;
- documente les choix et limites significatifs ;
- protège les accès et données confiés ;
- signale les dépendances et coûts récurrents connus ;
- prépare la recette et la réversibilité ;
- réoriente lorsque le besoin dépasse son périmètre.

## 17.6 Responsabilités des fournisseurs

Le registrar, l’hébergeur, la messagerie, l’outil d’analyse et les API sont régis par leurs contrats. Claynum aide à les sélectionner et à les configurer, mais ne se substitue pas à eux pour leurs engagements de disponibilité, de conservation ou de support.

> **SCHÉMA À CRÉER ET INSÉRER**  
> Intitulé : Carte des responsabilités d’une prestation  
> Objectif : visualiser les frontières entre Claynum, client, fournisseur et spécialiste  
> Éléments : décisions, réalisation, contrats tiers, conformité, exploitation, support  
> Type : matrice ou diagramme en couloirs

# 18. Modèles et annexes opérationnelles

## 18.1 Fiche de qualification initiale

### Identification

- [ ] Client, activité et coordonnées renseignés
- [ ] Décideur et référent métier identifiés
- [ ] Objectif formulé comme un résultat observable
- [ ] Utilisateurs, rôles et équipements recensés
- [ ] Volumes actuels et prévisionnels estimés
- [ ] Données et sensibilité qualifiées
- [ ] Services, comptes et prestataires existants inventoriés
- [ ] Contraintes de délai, budget et réglementation signalées
- [ ] Indisponibilité et perte de données tolérables discutées
- [ ] Décision de prise en charge formalisée

### Questions de cadrage

| Question | Réponse à renseigner |
|---|---|
| Quel problème concret doit être résolu ? | |
| Qui utilisera la solution et pour faire quoi ? | |
| Quelles données seront collectées ou importées ? | |
| Que se passe-t-il si le service est indisponible une journée ? | |
| Quelle solution ou procédure existe aujourd’hui ? | |
| Quels abonnements et coûts récurrents sont acceptables ? | |
| Qui validera le résultat ? | |

## 18.2 Grille de sensibilité des données

| Niveau | Exemples | Mesures minimales | Décision Claynum |
|---|---|---|---|
| Public | contenus destinés au site | intégrité, sauvegarde, publication contrôlée | prise en charge standard |
| Interne | procédures, tarifs non publics | contrôle d’accès, sauvegarde, partage limité | prise en charge standard avec inventaire |
| Personnel courant | contacts, clients, comptes utilisateurs | minimisation, information, droits, chiffrement des échanges | prise en charge avec cadre RGPD |
| Sensible ou réglementé | santé, infractions, secret critique, grande échelle | analyse renforcée, exigences sectorielles, sécurité spécialisée | partenariat, limitation ou refus |

## 18.3 Fiche de cadrage d’une prestation

La fiche comporte au minimum :

- contexte et objectif ;
- périmètre inclus ;
- éléments explicitement exclus ;
- utilisateurs et rôles ;
- données et traitements ;
- architecture ou services envisagés ;
- livrables ;
- planning et dépendances ;
- responsabilités ;
- critères de recette ;
- coûts récurrents ;
- maintenance et réversibilité ;
- hypothèses et réserves.

## 18.4 Matrice des responsabilités à joindre au devis

| Élément | Claynum | Client | Fournisseur ou partenaire |
|---|---|---|---|
| Décision | propose et alerte | décide | conseille sur son domaine |
| Souscription | accompagne | souscrit et paie | fournit le service |
| Réalisation | réalise son lot | fournit et valide | réalise son lot |
| Exploitation | selon contrat | responsable par défaut | exploite sa plateforme |
| Conformité | traduit techniquement | responsable de l’activité | conseil spécialisé si requis |
| Réversibilité | prépare et remet | réceptionne et conserve | fournit les exports prévus |

## 18.5 Procès-verbal de recette

Projet : à renseigner  
Version : à renseigner  
Date : à renseigner  
Participants : à renseigner

| Scénario | Résultat attendu | Résultat obtenu | Statut | Observation |
|---|---|---|---|---|
| Parcours principal | | | conforme / réserve / non conforme | |
| Gestion des erreurs | | | conforme / réserve / non conforme | |
| Droits d’accès | | | conforme / réserve / non conforme | |
| Import ou export | | | conforme / réserve / non conforme | |
| Sauvegarde ou restauration | | | conforme / réserve / non conforme | |

La validation indique les réserves, le délai de correction convenu et la décision de mise en service.

## 18.6 Fiche de remise des accès

- [ ] Registrar et domaine remis
- [ ] Gestion DNS remise
- [ ] Hébergement remis
- [ ] Messagerie et comptes administrateurs remis
- [ ] Dépôt de code ou archive remis
- [ ] Outil de mesure d’audience remis
- [ ] Services externes et API inventoriés
- [ ] Méthodes de récupération vérifiées
- [ ] Authentification multifacteur activée
- [ ] Secrets temporaires remplacés
- [ ] Accès Claynum révoqués ou maintenus selon contrat

Les secrets sont transmis par un canal adapté et ne sont pas consignés en clair dans cette fiche.

## 18.7 Inventaire technique d’une solution

| Catégorie | Élément à renseigner |
|---|---|
| Domaine principal et variantes | nom, titulaire, registrar, échéance |
| DNS | gestionnaire, serveurs de noms, export de zone |
| Hébergement | fournisseur, offre, région, échéance |
| Code | dépôt, branche ou version livrée, licence |
| Base de données | technologie, version, emplacement, sauvegarde |
| Stockage | type, emplacement, quota, rétention |
| Messagerie | fournisseur, domaine, administrateurs |
| Services externes | API, finalité, compte titulaire, coût |
| Sécurité | MFA, secrets, comptes administrateurs, journaux |
| Exploitation | responsable, mises à jour, alertes, maintenance |

## 18.8 Liste de contrôle avant mise en production

- [ ] Version à publier identifiée et archivée
- [ ] Sauvegarde préalable réalisée et contrôlée
- [ ] Retour arrière défini
- [ ] Paramètres et secrets de production vérifiés
- [ ] Comptes et droits vérifiés
- [ ] HTTPS et DNS contrôlés
- [ ] Données de test retirées
- [ ] Journaux configurés sans données excessives
- [ ] Sauvegardes de production planifiées
- [ ] Parcours essentiels testés
- [ ] Mentions et informations sur les données publiées
- [ ] Client informé de la mise en service
- [ ] Responsable de l’exploitation désigné

## 18.9 Liste de contrôle de fin de prestation

- [ ] Livrables validés
- [ ] Réserves et corrections restantes consignées
- [ ] Code, données et documents remis
- [ ] Abonnements et coûts récurrents rappelés
- [ ] Échéances de renouvellement connues
- [ ] Accès administrateurs récupérés par le client
- [ ] Accès temporaires révoqués
- [ ] Copies de travail traitées
- [ ] Maintenance ou absence de maintenance confirmée
- [ ] Point de contact futur précisé

## 18.10 Inventaire des schémas à produire

La seconde passe documentaire doit reprendre chaque marqueur du présent référentiel et produire une série cohérente. Le style graphique devra privilégier des libellés courts, peu de couleurs et un niveau de détail adapté aux clients non spécialistes.

| N° | Schéma | Chapitre | Priorité |
|---|---|---:|---|
| 1 | Place du référentiel dans la prestation | 1 | moyenne |
| 2 | Arbre de décision de prise en charge | 3 | haute |
| 3 | Acteurs d’un nom de domaine | 5 | haute |
| 4 | Du nom au serveur web | 6 | haute |
| 5 | Enregistrements d’une zone DNS | 6 | haute |
| 6 | Parcours d’un courriel | 7 | moyenne |
| 7 | Chaîne de publication | 8 | haute |
| 8 | Architecture d’une application web | 10 | haute |
| 9 | De la maquette à la production | 10 | moyenne |
| 10 | Cycle de vie d’une donnée | 11 | moyenne |
| 11 | Défense en profondeur | 12 | moyenne |
| 12 | Rôles RGPD | 13 | haute |
| 13 | Cycle d’une prestation | 14 | haute |
| 14 | Réversibilité | 16 | moyenne |
| 15 | Carte des responsabilités | 17 | haute |

## 18.11 Glossaire

| Terme | Définition opérationnelle |
|---|---|
| API | interface permettant à deux logiciels d’échanger selon des règles définies |
| Base de données | système structuré de stockage, recherche et mise à jour de données |
| CNAME | enregistrement DNS déclarant qu’un nom est l’alias d’un autre |
| DKIM | signature appliquée aux courriels par le domaine émetteur |
| DMARC | politique de contrôle et de rapport sur l’authentification des courriels |
| DNS | système qui associe les noms de domaine aux services correspondants |
| Hébergeur | fournisseur de l’infrastructure sur laquelle un site ou une application fonctionne |
| HTTPS | échange HTTP protégé par TLS entre le navigateur et le serveur |
| MFA | authentification utilisant au moins deux facteurs distincts |
| MX | enregistrement DNS désignant les serveurs de réception des courriels |
| Registrar | bureau d’enregistrement auprès duquel un domaine est souscrit et géré |
| Registre | organisme gérant une extension de domaine, par exemple l’Afnic pour .fr |
| Réversibilité | capacité à reprendre ou transférer comptes, code, configuration, données et documentation |
| SPF | règle DNS indiquant les systèmes autorisés à émettre pour un domaine |
| Sous-traitant RGPD | organisme traitant des données personnelles pour le compte d’un responsable de traitement |
| TTL | durée pendant laquelle une réponse DNS peut rester en cache |

## 18.12 Sources institutionnelles de référence

Les sources suivantes ont été consultées pour la version 1.0. Elles doivent être vérifiées à nouveau avant toute utilisation contractuelle ou décision sensible.

- Afnic — Guide pratique du titulaire d’un nom de domaine en .fr
- Afnic — Foire aux questions sur les noms de domaine
- CNIL — Guide de la sécurité des données personnelles
- CNIL — Cookies et traceurs : que dit la loi ?
- CNIL — Responsable de traitement et sous-traitant : identifier son rôle
- CNIL — Sécurité : gérer la sous-traitance
- CNIL — Sécurité : tracer les opérations
- ANSSI — Catalogue des guides et services cyber
- Entreprendre.Service-Public.fr — Mentions obligatoires sur un site professionnel
- Entreprendre.Service-Public.fr — Obligations en matière de protection des données

## 18.13 Statut du document

Ce référentiel décrit le cadre de travail visé par Claynum à la date de sa version. Il doit être adapté à chaque prestation. Il ne constitue ni un engagement de service général, ni une certification, ni un avis juridique.

Les schémas signalés par des marqueurs seront conçus et insérés lors d’une seconde passe. Après cette étape, une revue finale vérifiera la cohérence entre texte, schémas, matrices et modèles opérationnels.
