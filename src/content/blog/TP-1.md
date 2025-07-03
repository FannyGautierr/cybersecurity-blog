---
title: 'Tp1 : Attaque contre France Travail'
description: 'Cyberattaque en 2024 : '
pubDate: 'June 30 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---
# Cyberattaque de France Travail : Analyse d'un incident majeur de cybersécurité

![France Travail Cyberattaque](https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg)
## Vue d'ensemble de l'incident

En mars 2024, France Travail (anciennement Pôle emploi) et Cap emploi ont été victimes d'une cyberattaque majeure ayant entraîné l'exfiltration des données personnelles de 43 millions de personnes. [L'attaque s'est déroulée entre le 6 février et le 5 mars 2024](https://www.cybermalveillance.gouv.fr/tous-nos-contenus/actualites/violation-de-donnees-personnelles-france-travail-formulaire-lettre-plainte-202403), avant d'être détectée par France Travail dans la semaine du 13 mars.

Cette cyberattaque constitue **l'une des plus importantes fuites de données de l'histoire française** en termes de volume d'informations compromises, surpassant même certains incidents majeurs dans le secteur privé.

>" C’est la plus importante cyberattaque de l’histoire de France Travail et même l’une des plus graves à l’échelle française en termes de quantité de données compromises."
>
>[Source : France Bleu](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217)

![Données compromises](https://www.radiofrance.fr/s3/cruiser-production-eu3/2024/05/5fa6f9bb-0914-4f91-90c0-c68b46c69ce3/860_sc_photo-4-mail-cyberattaque.jpg)

## Analyse technique de l'attaque

### Vecteur d'intrusion initial

[L'attaque a débuté par une "usurpation d'identité de conseillers Cap emploi"](https://www.francebleu.fr/infos/societe/france-travail-43-millions-de-personnes-potentiellement-concernees-par-une-cyberattaque-8070716), technique d'ingénierie sociale sophistiquée. Suite à cette compromission initiale, [France Travail a détecté des "requêtes suspectes" dans ses systèmes](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article).

Cette méthode révèle plusieurs vulnérabilités organisationnelles :
- **Faiblesse dans l'authentification** des partenaires externes (Cap emploi)
- **Manque de contrôles d'accès** suffisamment robustes
- **Surveillance insuffisante** des activités anormales en temps réel

### Techniques d'exfiltration

Bien que les détails techniques précis n'aient pas été communiqués publiquement pour des raisons de sécurité, l'analyse de la chronologie révèle :

- **Durée de persistance** : Près d'un mois (6 février au 5 mars 2024)
- **Volume massif** : 43 millions d'enregistrements extraits
- **Discrétion de l'opération** : L'attaque n'a été détectée qu'après plusieurs semaines

Cette persistance prolongée suggère une **attaque sophistiquée** avec des capacités d'évasion et de camouflage avancées.

## Données compromises et impact

### Typologie des données exfiltrées

[Les données personnelles d'identification exposées incluent : nom et prénom, date de naissance, numéro de sécurité sociale, identifiant France Travail, adresses mail et postales, et numéros de téléphone](https://www.cnil.fr/fr/france-travail-la-cnil-enquete-sur-la-fuite-de-donnees-et-donne-des-conseils-pour-se-proteger).

**Points positifs de la sécurité :**
[Les mots de passe et les coordonnées bancaires ne sont pas concernés par cet acte de cybermalveillance](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article).

### Périmètre des victimes

[La base de données compromise contient les informations des personnes actuellement inscrites, des personnes précédemment inscrites au cours des 20 dernières années ainsi que des personnes non inscrites sur la liste des demandeurs d'emploi mais ayant un espace candidat sur francetravail.fr](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article).

Cette étendue révèle une **centralisation importante des données** sur plusieurs décennies, amplifiant l'impact de la brèche.

## Vulnérabilités systémiques identifiées

![Historique des failles](https://geimage.newstank.fr/image/cms/a37ad3af75c18baea197f822aa35dfd2/france-travail-impact-effets-cyberattaque.jpg?fm=browser&crop=0%2C38%2C800%2C450&w=1200&h=627&s=ff4a18c7711edac70c8a1d0ad4ca1e6e)

### Historique de failles de sécurité

[France Travail n'en était pas à sa première cyberattaque. Au moins deux autres piratages avaient visé l'organisme ces dernières années](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217), posant la question de sa responsabilité en matière de cybersécurité.

[En 2021, un incident avait déjà permis l'extraction d'environ 50 000 identités par un employé interne](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217), révélant des failles dans le contrôle des accès internes.

### Défaillances organisationnelles

L'analyse des incidents précédents révèle plusieurs problématiques structurelles :

- **Contrôles d'accès insuffisants** : Un employé pouvait accéder à des volumes massifs de données
- **Monitoring défaillant** : Les extractions répétées n'ont pas déclenché d'alertes
- **Segmentation réseau** : Accès trop large depuis les postes de travail
- **Sensibilisation** : Formation insuffisante à la sécurité

## Conséquences en cybersécurité

![Risques cybersécurité](https://bigmedia.bpifrance.fr/sites/default/files/inline-images/extrait%20info.PNG)

### Risques immédiats

[Les conséquences potentielles concernent les différentes formes d'hameçonnage (phishing), de tentatives d'escroqueries ou d'usurpation d'identité](https://www.cybermalveillance.gouv.fr/tous-nos-contenus/actualites/violation-de-donnees-personnelles-france-travail-formulaire-lettre-plainte-202403).

**Scénarios d'attaque probables :**
- **Spear phishing** ciblé utilisant les données personnelles
- **Ingénierie sociale** renforcée par la connaissance des victimes
- **Usurpation d'identité** facilitée par la richesse des informations
- **Couplage avec d'autres fuites** pour des attaques sophistiquées

### Impact à long terme

[Il est possible que les données ayant fait l'objet de la violation soient couplées, par des acteurs malveillants, à d'autres informations provenant de fuites de données antérieures](https://www.cnil.fr/fr/france-travail-la-cnil-enquete-sur-la-fuite-de-donnees-et-donne-des-conseils-pour-se-proteger).

## Réponse incident et mesures correctives

### Actions immédiates

[France Travail a procédé à une notification auprès de la CNIL et a déposé plainte auprès des autorités judiciaires](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article). [Une enquête préliminaire a été ouverte par le Parquet de Paris et confiée à la Brigade de Lutte Contre la Cybercriminalité](https://www.cybermalveillance.gouv.fr/tous-nos-contenus/actualites/violation-de-donnees-personnelles-france-travail-formulaire-lettre-plainte-202403).

### Investigations CNIL

[La présidente de la CNIL a décidé de mener très rapidement des investigations afin de déterminer notamment si les mesures de sécurité mises en œuvre préalablement à l'incident et en réaction à celui-ci étaient appropriées au regard des obligations du RGPD](https://www.cnil.fr/fr/france-travail-la-cnil-enquete-sur-la-fuite-de-donnees-et-donne-des-conseils-pour-se-proteger).

### Mesures de renforcement

[Dès la connaissance avérée de cette intrusion, France Travail a pris des mesures complémentaires avec le réseau Cap emploi pour renforcer les dispositifs de protection des accès aux applicatifs par les partenaires](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article).

## Enseignements pour la cybersécurité française

**Modernisation en cours :**
[Face aux critiques, France Travail affirme avoir désormais recours fréquemment à des audits externes et à des hackeurs éthiques qui ont pour mission de "tester nos défenses. Et s'ils découvrent des failles, nous les réparons"](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217). [L'organisme reconnaît un "travail permanent" pour sécuriser tous ses sites, certains mis en ligne "il y a 10 ou 15 ans"](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217).

Cette cyberattaque illustre plusieurs défis majeurs :

1. **Vulnérabilité des services publics** face aux cybermenaces
2. **Nécessité de moderniser** les infrastructures de sécurité
3. **Importance du facteur humain** dans la cybersécurité
4. **Besoin de coordination** entre organismes publics et partenaires

[Face à la menace de cyber attaques qui pèse de plus en plus sur les entreprises et organisations au niveau national comme européen, nous nous devons de renforcer en continu nos dispositifs de protection, procédures et consignes](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article).

## Conclusion

L'incident de France Travail démontre l'urgence de moderniser la cybersécurité des administrations publiques françaises. Au-delà des aspects techniques, cette cyberattaque souligne l'importance cruciale d'une approche holistique incluant la gouvernance, les processus, et la sensibilisation humaine.

La gestion de crise a été globalement conforme aux bonnes pratiques (notification rapide, communication transparente, dispositif de plainte simplifié), mais l'incident révèle des failles structurelles qui nécessitent des investissements significatifs en cybersécurité.

---
**Sources principales :**
- **CNIL** - [Enquête sur la fuite de données France Travail](https://www.cnil.fr/fr/france-travail-la-cnil-enquete-sur-la-fuite-de-donnees-et-donne-des-conseils-pour-se-proteger)
- **Cybermalveillance.gouv.fr** - [Violation de données personnelles](https://www.cybermalveillance.gouv.fr/tous-nos-contenus/actualites/violation-de-donnees-personnelles-france-travail-formulaire-lettre-plainte-202403)
- **France Travail** - [Communiqué officiel de cyberattaque](https://www.francetravail.org/accueil/communiques/2024/france-travail-et-cap-emploi-victimes-dune-cyberattaque.html?type=article)
- **France Bleu - Cellule Investigation** - [Enquête approfondie sur les vulnérabilités](https://www.francebleu.fr/infos/economie-social/cyberattaque-a-france-travail-la-direction-avait-ete-informee-d-une-faiblesse-dans-la-securite-2197217)
- **NextINpact** - [Analyse technique du volume réel](https://next.ink/132025/france-travail-un-piratage-limite-a-3-des-43-millions-des-victimes-potentielles/)

---

**Documents officiels :**
- [Réponses officielles de France Travail](https://www.calameo.com/read/006296452bef2590cbe29) (suite à l'enquête)
- [Réponses de Majorel](https://www.calameo.com/read/0062964526fc69e224312) (prestataire impliqué en 2023)
- [Jugement tribunal prud'hommes Amiens](https://www.calameo.com/read/00629645280abd6b04799) (incident 2021)

---