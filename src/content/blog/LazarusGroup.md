---
title: "Lazarus Group - Les pirates de l'économie nord-coréenne"
description: "Analyse du Lazarus Group : groupe cybercriminel nord-coréen évoluant de l'espionnage vers les attaques financières"
pubDate: 'Jul 3 2025'
heroImage: 'https://c.files.bbci.co.uk/CFE1/production/_118971235_bbc_tlh_arta1-nc-1.png'
---

## 1. Identification du groupe

**Nom principal :** Lazarus Group  
**Aliases :** Guardians of Peace, Whois Team, Hidden Cobra, ZINC, Diamond Sleet, APT38 (sous-groupe)   
**Origine :** Corée du Nord   
**Affiliation :** Reconnaissance General Bureau (RGB) - bureau principal de renseignement nord-coréen   
**Nom interne :** 414 Liaison Office (selon un transfuge nord-coréen)   
**Motivation :** Financière et géopolitique, financement du programme d'armement nord-coréen

## 2. Historique des opérations

### **Timeline des attaques majeures :**

**2009 :** Première attaque majeure le 4 juillet avec l'Opération Troy - Attaque DDoS contre des sites américains et sud-coréens   
**2013 :** Attaque DarkSeoul contre des banques et médias sud-coréens  
**2014 :** Attaque contre Sony Pictures Entertainment (15 millions $ de dommages selon Sony)   
**2016 :** Tentative de vol de 951 millions $ à la Banque du Bangladesh, 81 millions $ volés avec succès   
**2017 :** Diffusion du ransomware WannaCry (attribué par Symantec)   
**2018 :** Attaques FASTCash contre les DAB pour retirer frauduleusement des espèces   
**2017-présent :** Série continue d'attaques contre les échanges de cryptomonnaies   
**2022 :** Vol de 620 millions $ du Ronin Network (Axie Infinity)   
**2023 :** Responsable de plus de 300 millions $ de pertes dans les incidents de piratage crypto   
**2025 :** Attaque présumée contre Bybit - 1,5 milliard $ volés 

## 3. Arsenal technique

### **Malwares et outils signatures :**
- **Mydoom et Dozer :** Utilisés dans les premières attaques DDoS de 2009 
- **Malware BazarLoader :** Pour l'infiltration initiale
- **Outils légitimes détournés :** Exploitation d'outils de simulation d'adversaire comme Cobalt Strike 
- **Custom malware :** Développement de trojans d'accès distant (RAT) personnalisés 

### **Tactiques spécialisées :**
- **Social engineering :** Sophistiqué, utilisant la tromperie et la coercition pour obtenir mots de passe et clés privées 
- **Exploitation de vulnérabilités :** Hangul (logiciel de traitement de texte sud-coréen), Log4J 
- **Spear-phishing :** Leurres malveillants envoyés aux étudiants sud-coréens et utilisateurs d'échanges crypto 
- **Attaques supply chain :** Compromission de logiciels légitimes

### **Évolution technique :**
Le groupe moderne développe des malwares personnalisés et possède la capacité de mener des cyberattaques hautement sophistiquées 

## 4. Victimologie

### **Secteurs ciblés :**

**Phase espionnage (2009-2013) :**
- Gouvernement et militaire sud-coréens
- Infrastructures critiques

**Phase destructrice (2014-2016) :**
- Industrie du divertissement (Sony Pictures) 
- Système bancaire international (Bangladesh Bank) 

**Phase financière (2016-présent) :**
- Échanges de cryptomonnaies et utilisateurs 
- Institutions financières dans 11 pays (Bangladesh, Inde, Mexique, Pakistan, Philippines, Corée du Sud, Taïwan, Turquie, Chili, Vietnam) 
- Systèmes SWIFT et institutions financières 

### **Motivation géographique :**
- **Priorité :** Corée du Sud (ennemi traditionnel)
- **Expansion :** Cibles financières mondiales pour financer le régime

## 5. Particularités

### **Évolution unique :**
Passage de l'espionnage et des attaques destructrices vers la cybercriminalité financière motivée par le besoin de devises étrangères face aux sanctions internationales 

### **Structure organisationnelle :**
Lazarus comprend deux unités principales : BlueNorOff (APT38) - groupe financièrement motivé responsable des transferts illégaux 

### **Formation et recrutement :**
Les hackers nord-coréens sont envoyés professionnellement à Shenyang, Chine pour formation spéciale. Éducation nationale à l'Université de technologie Kim Chaek, Université Kim Il Sung et Université Moranbong 

### **Spécialisation crypto :**
Le groupe emploie une combinaison de tactiques qui évoluent dans le temps, exploitant les vulnérabilités traditionnelles et spécifiques au Web3 

### **Modèle économique :**
Les attaques visent à stimuler l'économie nord-coréenne affaiblie et à financer les ambitions nationales comme le développement de missiles et d'armes nucléaires 

## 6. Indicateurs de compromission

### **Comportements caractéristiques :**
- Similarités techniques avec WannaCry et attaques Sony Pictures
- Réutilisation de code (bien que cela puisse être un "false flag") 
- Ciblage spécifique des institutions financières et crypto

### **Artefacts techniques :**
- Exploitation d'outils légitimes détournés
- Code personnalisé sophistiqué nécessitant des ressources importantes 
- Communications vers l'infrastructure nord-coréenne

### **Patterns d'attaque :**
- Préparation extensive (plus d'un an dans les systèmes Sony) 
- Combinaison d'espionnage et destruction
- Focus sur l'exfiltration de grandes sommes

## 7. Contre-mesures

### **Protection financière :**
- Surveillance renforcée des transactions SWIFT
- Authentification multi-couches pour les transferts
- Monitoring des échanges de cryptomonnaies

### **Sécurité technique :**
- Patches immédiat des vulnérabilités (Log4J, systèmes de paiement)
- Segmentation des systèmes financiers critiques
- Protection contre le social engineering

### **Intelligence des menaces :**
- Surveillance des sanctions : éviter les paiements qui pourraient violer les sanctions contre la Corée du Nord 
- Partage d'informations avec les institutions financières
- Monitoring des adresses Bitcoin/crypto connues

### **Réponse institutionnelle :**
Les États-Unis ont imposé des sanctions ciblant les trois groupes (Lazarus, Bluenoroff, Andariel) et offert des récompenses allant jusqu'à 15 millions $ pour des informations 

### **Prévention spécialisée :**
- Formation anti-phishing spécifique au secteur crypto
- Validation des smart contracts et audits de sécurité DeFi
- Surveillance des cross-chain bridges

## Sources

- [The Lazarus group: North Korean scourge for +10 years | NCC Group](https://www.nccgroup.com/us/the-lazarus-group-north-korean-scourge-for-plus10-years/)
- [Lazarus Group - Wikipedia](https://en.wikipedia.org/wiki/Lazarus_Group)
- [Treasury Sanctions North Korean Malicious Cyber Groups | U.S. Treasury](https://home.treasury.gov/news/press-releases/sm774)
- [Lazarus Group: North Korea's Elite Cyber Threat Actor | SecMaster](https://thesecmaster.com/blog/lazarus-group)
- [Lazarus Group: The Hackers Behind Bybit's $1.5B Exploit | Hacken](https://hacken.io/discover/lazarus-group/)
- [U.S. Sanctions North Korean Group Behind WannaCry | Threatpost](https://threatpost.com/us-sanctions-north-korea-wannacry-sony-hacks/148351/)
- [North Korean Regime-Backed Programmer Charged | DOJ](https://www.justice.gov/archives/opa/pr/north-korean-regime-backed-programmer-charged-conspiracy-conduct-multiple-cyber-attacks-and)
- [Three North Korean Military Hackers Indicted | DOJ](https://www.justice.gov/archives/opa/pr/three-north-korean-military-hackers-indicted-wide-ranging-scheme-commit-cyberattacks-and)
- [A History of the Lazarus Group | Halborn](https://www.halborn.com/blog/post/a-history-of-the-lazarus-group-north-korea-s-notorious-cyber-actors)