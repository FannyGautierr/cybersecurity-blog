---
title: "NotPetya (2017) - L'arme cyberguerre déguisée en ransomware"
description: 'Analyse de NotPetya : cyberattaque destructrice attribuée à la Russie, causant 10 milliards de dollars de dommages'
pubDate: 'Jul 2 2025'
heroImage: 'https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Petya.Random.png/250px-Petya.Random.png'
---

## Quelle est la vulnérabilité exploitée ?

NotPetya a exploité plusieurs vulnérabilités :
- CVE-2017-0144 : Vulnérabilité EternalBlue dans SMB (identique à WannaCry) 
- CVE-2017-0145 : Vulnérabilité EternalRomance dans SMB 
- Compromission de M.E.Doc : Logiciel de comptabilité ukrainien utilisé comme vecteur initial 

## Comment l'attaque s'est-elle déroulée ?

L'attaque du 27 juin 2017  était particulièrement sophistiquée :

1. **Préparation** : Compromission du système de mise à jour de M.E.Doc depuis avril 2017 
2. **Injection** : Installation d'une backdoor dans les serveurs de M.E.Doc 
3. **Déploiement** : Distribution de NotPetya via une fausse mise à jour M.E.Doc
4. **Propagation** : Utilisation d'EternalBlue et de Mimikatz pour se propager 
5. **Destruction** : Chiffrement irréversible des données (pas de vraie récupération possible) 
6. **Expansion mondiale** : Propagation depuis l'Ukraine vers le monde entier 

## Qui a été touché ?

**Ukraine (80% des victimes)** :
- Banques (Oschadbank, Ukrsotsbank), Médias (STB, ICTV), Transport (Métro de Kiev, aéroport), Énergie (centrales électriques) 

**International** :
- Maersk : 250-300 millions $ de pertes 
- FedEx (TNT Express) : 400 millions $ de pertes 
- Merck & Co : 870 millions $ de pertes 
- Mondelez : 100 millions $ de pertes 

## Quels ont été les impacts ?

- Dommages économiques : 10 milliards $ selon l'évaluation de la Maison Blanche 
- Perturbation des infrastructures : Système de monitoring de Chernobyl hors ligne 
- **Paralysie logistique** : Maersk immobilisé pendant des semaines 
- **Impact géopolitique** : Première cyberguerre moderne documentée, attribuée au GRU russe 
- **Destruction de données** : Perte irréversible de données critiques

## Quel coût estimé ?

- **Petite entreprise** : 500 000 € à 2 000 000 € (reconstruction complète des systèmes)
- **Moyenne entreprise** : 5 000 000 € à 20 000 000 € (perte opérationnelle majeure)
- **Grande entreprise** : 50 000 000 € à 1 000 000 000 € (comme démontré par Maersk, FedEx, Merck)

## Comment s'en protéger ?

1. **Patchs de sécurité** : Installation immédiate des correctifs MS17-010 
2. **Segmentation réseau** : Isolation des systèmes critiques
3. **Gestion des fournisseurs** : Vérification de la sécurité des logiciels tiers
4. **Sauvegardes offline** : Copies de sauvegarde déconnectées du réseau
5. **Surveillance réseau** : Détection des mouvements latéraux
6. **Plan de continuité** : Procédures de fonctionnement sans systèmes IT

## Pourquoi est-ce difficile à éviter ?

- Vecteur d'infection légitime : M.E.Doc était un logiciel obligatoire en Ukraine 
- **Propagation automatique** : Exploitation de vulnérabilités pour se propager 
- Objectif destructeur : Pas de vraie récupération possible même en payant 
- Sophistication étatique : Attaque menée par des acteurs étatiques (GRU russe) 
- Vitesse de propagation : Infection complète en quelques minutes 
- Absence de kill switch : Contrairement à WannaCry, aucun moyen d'arrêt 

## Dans le contexte de votre entreprise, que feriez-vous ?

1. **Audit de vulnérabilités critique** : Vérification immédiate de toutes les failles SMB
2. **Plan de continuité robuste** : Capacité de fonctionner sans IT pendant des semaines
3. **Stratégie de sauvegarde 3-2-1** : 3 copies, 2 supports différents, 1 offline
4. **Évaluation géopolitique** : Considération des risques selon la zone géographique
5. **Tests de destruction** : Simulation de perte complète des systèmes
6. **Assurance cyber warfare** : Couverture spécifique pour les actes de cyberguerre
7. **Intelligence des menaces** : Veille sur les tensions géopolitiques
8. **Isolation des systèmes critiques** : Air gap pour les systèmes les plus sensibles

## Sources

- [2017 Ukraine ransomware attacks - Wikipedia](https://en.wikipedia.org/wiki/2017_Ukraine_ransomware_attacks)
- [Petya Ransomware | CISA](https://www.cisa.gov/news-events/alerts/2017/07/01/petya-ransomware)
- [What are Petya and NotPetya? | Cloudflare](https://www.cloudflare.com/learning/security/ransomware/petya-notpetya-ransomware/)
- [Petya (malware family) - Wikipedia](https://en.wikipedia.org/wiki/Petya_(malware_family))
- [What is NotPetya? 5 Fast Facts | Security Encyclopedia](https://www.hypr.com/security-encyclopedia/notpetya)
- [Email breach chronicles: The NotPetya catastrophe | Zoho](https://www.zoho.com/workplace/articles/notpetya-cyberattack.html)
- [How the NotPetya attack is reshaping cyber insurance | Brookings](https://www.brookings.edu/articles/how-the-notpetya-attack-is-reshaping-cyber-insurance/)
- [NotPetya (2017) - International cyber law: interactive toolkit](https://cyberlaw.ccdcoe.org/wiki/NotPetya_(2017))
- [Throwback Attack: How NotPetya Took Down Maersk | Control Engineering](https://www.controleng.com/throwback-attack-how-notpetya-accidentally-took-down-global-shipping-giant-maersk/)