---
title: 'Target (2013) - La faille qui a révolutionné la sécurité retail'
description: 'Analyse du piratage Target : 110 millions de clients compromis via un fournisseur HVAC, révélant les risques tiers'
pubDate: 'Jul 2 2025'
heroImage: 'https://krebsonsecurity.com/wp-content/uploads/2014/01/targetsmash.jpg'
---

## Quelle est la vulnérabilité exploitée ?

L'attaque Target n'a pas exploité une CVE spécifique mais plusieurs faiblesses :
- Compromission d'un fournisseur tiers : Fazio Mechanical Services (HVAC) 
- **Segmentation réseau insuffisante** : Accès du fournisseur au réseau corporatif
- **Malware POS** : Installation de logiciels malveillants sur les terminaux de paiement
- Défaillance de surveillance : Alertes ignorées malgré la détection par FireEye 

## Comment l'attaque s'est-elle déroulée ?

L'attaque s'est déroulée en plusieurs phases entre novembre et décembre 2013 :

1. **Phishing initial** : Email malveillant envoyé à Fazio Mechanical en septembre 2013 
2. **Compromission du fournisseur** : Vol des identifiants réseau de Fazio 
3. **Accès latéral** : Utilisation des credentials pour accéder au réseau Target le 15 novembre
4. **Installation malware** : Déploiement de malware sur les systèmes POS
5. **Collecte de données** : Capture des données de cartes de crédit en mémoire
6. **Exfiltration** : Transfert des données vers des serveurs externes le 30 novembre
7. **Découverte** : Le DoJ alerte Target de l'intrusion le 12 décembre 

## Qui a été touché ?

- 110 millions de clients au total : 40 millions de cartes de crédit/débit compromises, 70 millions de données personnelles (noms, adresses, téléphones, emails) 
- Période d'impact : 27 novembre - 15 décembre 2013 (période des fêtes) 
- **Zones géographiques** : Tous les magasins Target aux États-Unis

## Quels ont été les impacts ?

- Impact financier direct : 162 millions $ de coûts immédiats 
- Règlements judiciaires : 18,5 millions $ de settlement multiétatique 
- Perte de confiance client : Baisse de 10% de la fréquentation (33% des foyers) 
- Impact sur les ventes : Chute de 46% des profits Q4 2013 
- Changements de direction : Démission du CEO et du CIO en 2014 
- **Coûts de conformité** : Mise aux normes PCI-DSS renforcées

## Quel coût estimé ?

- **Petite entreprise** : 100 000 € à 500 000 € (investigation, notification, amendes)
- **Moyenne entreprise** : 1 000 000 € à 5 000 000 € (systèmes POS, expertise légale)
- **Grande entreprise** : 50 000 000 € à 500 000 000 € (impact réputationnel, class actions)

## Comment s'en protéger ?

1. **Gestion des accès tiers** : Contrôle strict des accès fournisseurs
2. **Segmentation réseau** : Isolation des systèmes de paiement 
3. **Chiffrement point-to-point** : Chiffrement des données dès la capture 
4. **Surveillance 24/7** : Monitoring avec réponse aux alertes 
5. **Tokenisation** : Remplacement des données sensibles par des tokens 
6. **Audit des fournisseurs** : Évaluation régulière de la sécurité des tiers
7. **Formation phishing** : Sensibilisation des partenaires

## Pourquoi est-ce difficile à éviter ?

- **Complexité des partenariats** : Multiples fournisseurs avec accès réseau 
- **Confiance excessive** : Accès privilégiés accordés sans contrôle suffisant
- **Chaîne de responsabilité** : Sécurité dépendante des pratiques des tiers 
- **Période critique** : Attaque pendant les fêtes (forte activité, vigilance réduite)
- Détection vs. Réaction : Outils de détection présents mais réponse inadéquate 
- **Legacy systems** : Systèmes POS souvent difficiles à sécuriser

## Dans le contexte de votre entreprise, que feriez-vous ?

1. **Audit des accès tiers** : Révision complète de tous les accès fournisseurs
2. **Architecture Zero Trust** : Principe de moindre privilège pour tous les accès
3. **Chiffrement bout-en-bout** : Sécurisation de toutes les données de paiement
4. **SOC opérationnel** : Centre de sécurité avec procédures de réponse aux incidents
5. **Contrats fournisseurs renforcés** : Clauses de sécurité et audits obligatoires
6. **Tests d'intrusion tiers** : Simulation d'attaques via les partenaires
7. **Plan de communication de crise** : Procédures de notification et gestion de crise
8. **Assurance cyber complète** : Couverture incluant les attaques via tiers
9. **Formation continue** : Sensibilisation étendue à l'écosystème de partenaires

## Sources

- [Warnings (& Lessons) of the 2013 Target Data Breach | Red River](https://redriver.com/security/target-data-breach)
- [What We Learned from Target's Data Breach 2013 | CardConnect](https://www.cardconnect.com/launchpointe/payment-trends/target-data-breach/)
- [Cyber Case Study: Target Data Breach | CoverLink Insurance](https://coverlink.com/cyber-liability-insurance/target-data-breach/)
- [The Target Breach: A Historic Cyberattack | Framework Security](https://www.frameworksec.com/post/the-target-breach-a-historic-cyberattack-with-lasting-consequences)
- [The Target Breach 10 Years Later | Security Info Watch](https://www.securityinfowatch.com/retail/article/53098895/the-target-breach-10-years-later)
- [The 2013 Target Data Breach | Mitratech](https://www.prevalent.net/blog/the-2013-target-data-breach-a-lasting-lesson-in-third-party-risk-management/)
- [Cyber Security Case Study: Target Data Breach | CEI](https://www.cei.com/about-cei/media-room/blog/cyber-security-targets-2013-data-breach)