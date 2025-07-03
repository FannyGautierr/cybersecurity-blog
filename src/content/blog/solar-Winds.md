---
title: "SolarWinds (2020) - La cyberattaque de la chaîne dapprovisionnement"
description: "Analyse de lattaque SolarWinds : supply chain attack sophistiquée attribuée à la Russie, compromettant 18 000 organisations"
pubDate: "Jul 2 2025"
heroImage: "https://les-yeux-du-monde.fr/wp-content/uploads/2021/02/SolarWinds-cyberattaque-espionnage-cyberse%CC%81curite%CC%81-Les-Yeux-du-Monde.jpg"
---

## Quelle est la vulnérabilité exploitée ?

L'attaque SolarWinds n'a pas exploité une vulnérabilité technique classique mais plutôt une vulnérabilité de la chaîne d'approvisionnement logicielle . Les attaquants ont compromis l'environnement de build de SolarWinds pour injecter le malware "Sunburst" dans les mises à jour légitimes d'Orion .

## Comment l'attaque s'est-elle déroulée ?

Cette attaque sophistiquée s'est déroulée sur plusieurs mois :

1. **Infiltration initiale** : Compromission de l'infrastructure SolarWinds commençant en septembre 2019 
2. **Test phase** : Injection de code de test dans le système de build 
3. **Déploiement malveillant** : Injection du malware Sunburst dans Orion à partir de février 2020 
4. **Distribution** : 18 000 clients reçoivent les mises à jour infectées 
5. **Activation sélective** : Le malware ne s'active que sur des cibles de haute valeur
6. **Découverte** : FireEye détecte l'intrusion en novembre 2020 et alerte SolarWinds 

## Qui a été touché ?

- 18 000 organisations ayant installé les mises à jour compromises 
- Agences gouvernementales US : Départements du Trésor, Commerce, Justice, Énergie 
- Entreprises Fortune 500 : Microsoft, Intel, Cisco et Deloitte, ainsi que le Pentagon 
- **Infrastructures critiques** : Systèmes de défense et de sécurité nationale
- **Fournisseurs cloud** : Impact en cascade sur leurs clients
- **Partenaires internationaux** : Gouvernements et entreprises alliés

## Quels ont été les impacts ?

- **Espionnage d'État** : Accès à des informations gouvernementales sensibles
- **Vol de propriété intellectuelle** : Secrets commerciaux et techniques
- **Compromission en cascade** : Accès aux clients des victimes primaires 
- **Perte de confiance** : Remise en question de la sécurité des logiciels tiers
- **Révision des politiques** : Nouvelles exigences de sécurité de la chaîne d'approvisionnement 

## Quel coût estimé ?

- **Petite entreprise** : 200 000 € à 1 000 000 € (investigation, remplacement)
- **Moyenne entreprise** : 2 000 000 € à 10 000 000 € (forensics, reconstruction)
- **Grande entreprise** : 50 000 000 € à 500 000 000 € (impact global, conformité)

*Note : Coûts souvent non quantifiables (espionnage, perte d'avantage concurrentiel) *

## Comment s'en protéger ?

1. **Sécurité de la chaîne d'approvisionnement** : Audit des fournisseurs critiques
2. **Vérification des signatures** : Contrôle d'intégrité des mises à jour
3. **Segmentation réseau** : Isolation des systèmes de monitoring
4. **Monitoring comportemental** : Détection d'activités anormales
5. **Zero Trust** : Vérification continue, même des systèmes "légitimes"
6. **Sauvegarde des configurations** : Possibilité de rollback rapide

## Pourquoi est-ce difficile à éviter ?

- **Confiance inhérente** : Les mises à jour étaient signées et légitimes 
- **Accès privilégié** : Orion a des accès étendus pour son fonctionnement normal 
- **Sophistication** : Attaque APT (Advanced Persistent Threat) très élaborée 
- **Détection complexe** : Comportement similaire aux activités légitimes
- **Chaîne de confiance** : Compromission en amont affecte tous les clients
- **Ressources limitées** : Difficile de vérifier tous les logiciels tiers

## Dans le contexte de votre entreprise, que feriez-vous ?

1. **Inventaire des logiciels tiers** : Cartographie complète des solutions critiques
2. **Programme de gestion des risques fournisseurs** : Évaluation continue de la sécurité
3. **Architecture Zero Trust** : Principe de vérification continue
4. **Surveillance comportementale** : Détection d'anomalies même sur systèmes "légitimes"
5. **Plan de réponse aux incidents** : Procédures spécifiques aux compromissions de chaîne d'approvisionnement
6. **Diversification des fournisseurs** : Éviter la dépendance à un fournisseur unique
7. **Collaboration sectorielle** : Partage d'informations de menaces avec les pairs
8. **Tests d'intrusion supply chain** : Simulation d'attaques de chaîne d'approvisionnement

## Sources

- [SolarWinds hack explained: Everything you need to know | TechTarget](https://www.techtarget.com/whatis/feature/SolarWinds-hack-explained-Everything-you-need-to-know)
- [SolarWinds Supply Chain Attack | Fortinet](https://www.fortinet.com/resources/cyberglossary/solarwinds-cyber-attack)
- [SolarWinds Cyberattack Demands Significant Response | U.S. GAO](https://www.gao.gov/blog/solarwinds-cyberattack-demands-significant-federal-and-private-sector-response-infographic)
- [SolarWinds Attack: Play by Play and Lessons Learned | Aqua](https://www.aquasec.com/cloud-native-academy/supply-chain-security/solarwinds-attack/)
- [Cyber Case Study: SolarWinds Supply Chain Cyberattack | Ollis/Akers/Arney](https://ollisakersarney.com/blog/cyber-case-study-solarwinds-supply-chain-cyberattack/)
- [SolarWinds and Software Supply Chain Attacks | BreachLock](https://www.breachlock.com/resources/blog/the-solarwinds-hack-and-the-arrival-of-software-supply-chain-attacks/)
- [What You Need To Know About the SolarWinds Supply-Chain Attack | SANS](https://www.sans.org/blog/what-you-need-to-know-about-the-solarwinds-supply-chain-attack/)
- [What is the SolarWinds Cyberattack? | Zscaler](https://www.zscaler.com/resources/security-terms-glossary/what-is-the-solarwinds-cyberattack)