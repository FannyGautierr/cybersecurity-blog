---
title: "BlackCat (ALPHV) - L'évolution du ransomware moderne"
description: "Analyse d'ALPHV BlackCat : groupe RaaS sophistiqué écrit en Rust, leader du ransomware moderne jusqu'à sa dissolution en 2024"
pubDate: 'Jul 3 2025'
heroImage: 'https://www.resecurity.com/uploads/post/118/118.jpg?af1f6d36c20f2863685809a8159066b1'
---

## 1. Identification du groupe

**Nom principal :** ALPHV BlackCat  
**Aliases :** BlackCat, ALPHV, Noberus, Ransom.Noberus   
**Origine :** Diverses nationalités (inconnues)   
**Type :** Ransomware-as-a-Service (RaaS)  
**Période d'activité :** Novembre 2021 - Février 2024   
**Particularité technique :** Premier ransomware écrit en langage Rust 

## 2. Historique des opérations

### **Timeline des attaques majeures :**

**Novembre 2021 :** Première apparition de BlackCat   
**Mars 2022 :** Environ 60 victimes documentées   
**Février 2023 :** Lancement de la variante "Sphynx" avec améliorations de vitesse et furtivité   
**Mai 2023 :** Plus de 350 victimes ciblées globalement   
**Juin 2023 :** Attaque contre Reddit (80 GB de données volées, demande de 4,5 millions $)   
**Septembre 2023 :** Attaques contre MGM Resorts et Caesars Entertainment via l'affilié Scattered Spider   
**Décembre 2023 :** Disruption FBI - saisie de sites web et libération d'outil de décryptage   
**Février 2024 :** Attaque contre Change Healthcare (plus de 100 millions d'individus compromis)   
**Mars 2024 :** Disparition après un paiement présumé de 22 millions $ d'Optum 

## 3. Arsenal technique

### **Innovation technologique :**
BlackCat est différent de la plupart des autres types de ransomware car il utilise le langage Rust, offrant de meilleures performances et protections de sécurité 

### **Chiffrement :**
Utilise plusieurs algorithmes de chiffrement forts : ChaCha20 pour le chiffrement du contenu des fichiers et RSA pour le chiffrement des clés. Parfois AES-256 

### **Tactiques d'accès initial :**
- Techniques d'ingénierie sociale avancées : les acteurs se font passer pour le personnel IT/helpdesk de l'entreprise 
- Malvertising et empoisonnement SEO pour distribuer des installateurs malveillants 
- Exploitation de credentials volés via des initial access brokers

### **Propagation et persistance :**
- Utilisation du malware botnet Emotet comme point d'entrée 
- Abus des Group Policy Objects (GPOs) pour distribuer le malware 
- Utilisation d'ExMatter pour voler les données sensibles 

### **Version 2.0 Sphynx :**
Mise à jour réécrite offrant de meilleures capacités d'évasion de défense et chiffrement des appareils Windows, Linux et instances VMware 

## 4. Victimologie

### **Secteurs les plus touchés :**
Depuis mi-décembre 2023, le secteur de la santé a été le plus victimisé (environ 70 victimes divulguées) 

### **Modèle d'affiliation :**
BlackCat opère comme plateforme RaaS, permettant aux autres cybercriminels d'utiliser son ransomware en échange d'une part des profits. Contrairement aux modèles RaaS typiques (70% aux affiliés), BlackCat offre 80-90% aux affiliés 

### **Victimes notables :**
- MGM Resorts : Attaque par l'affilié Scattered Spider 
- Caesars Entertainment : Autre cible majeure de Scattered Spider 
- UnitedHealth/Change Healthcare : L'affilié Notchy a revendiqué l'attaque 
- Reddit : 80 GB de données volées 

### **Impact global :**
Le FBI a identifié que les acteurs ALPHV/Blackcat ont compromis plus de 1 000 entités victimes aux États-Unis et ailleurs 

## 5. Particularités

### **Innovations du groupe :**

**Site de fuite public :** Premier groupe ransomware à créer un site de fuite de données public sur l'internet ouvert, contrairement aux sites dark web traditionnels 

**Triple extorsion :** Menaces de chiffrement, vol de données ET attaques DDoS pour ceux qui ne paient pas 

**Modèle économique attractif :** Le modèle de revenus agit comme un puissant outil publicitaire, générant un intérêt organique 

**Chiffrement intermittent :** Un des premiers groupes à supporter les modes de chiffrement intermittent 

### **Comportement post-disruption :**
Après l'action FBI de décembre 2023, encouragement des affiliés à cibler les hôpitaux 

### **Communication avec victimes :**
Utilisation d'URLs pour chat en direct avec les victimes pour transmettre les demandes 

## 6. Indicateurs de compromission

### **Artefacts fichiers :**
Extensions de fichiers chiffrés : .alphv, .onion, ou chaînes de caractères aléatoires 

### **Notes de rançon :**
Note de rançon généralement nommée "RECOVER-FILES.txt" 

### **Comportements système :**
- Suppression des volume shadow copies avec des commandes comme "vssadmin delete shadows" 
- Activité PowerShell inhabituelle, nouvelles tâches planifiées, connexions réseau inattendues 

### **Tactiques d'évasion :**
- Whitelisting d'applications comme Metasploit pour paraître légitimes 
- Effacement des logs sur le serveur Exchange après installation de malware sur le contrôleur de domaine 

## 7. Contre-mesures

### **Mesures préventives spécifiques :**

**Gestion des accès distants :**
Implémenter des contrôles d'application pour gérer et whitelister les programmes d'accès distant autorisés 

**Sécurité des bases de données :**
Savoir où résident toutes vos données est clé car c'est ce que recherche un attaquant 

**Formation et sensibilisation :**
Effectuer des sessions de formation régulières pour éduquer les employés sur les tactiques de phishing et méthodes d'ingénierie sociale utilisées par BlackCat 

### **Protections techniques :**

**Mises à jour et patchs :**
S'assurer que tous les systèmes, applications et appareils sont constamment mis à jour 

**Segmentation réseau :**
Implémenter la segmentation réseau pour limiter les mouvements latéraux 

**Sauvegardes robustes :**
Maintenir des sauvegardes régulières et chiffrées stockées hors ligne ou dans des formats immuables 

### **Détection et réponse :**
Les outils EDR modernes peuvent être efficaces contre le ransomware BlackCat s'ils sont correctement configurés et surveillés 

### **Évaluations continues :**
Vérifications de santé sécuritaire régulières : les évaluations et mises à jour continues garantissent que vos défenses restent fortes 

## Sources

- [#StopRansomware: ALPHV Blackcat | CISA](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-353a)
- [The Anatomy of a BlackCat Ransomware Attack | Sygnia](https://www.sygnia.co/blog/blackcat-ransomware/)
- [ALPHV Ransomware: Analyzing BlackCat | Picus Security](https://www.picussecurity.com/resource/blog/alphv-ransomware)
- [Reward for Information: ALPHV/Blackcat | U.S. State Department](https://www.state.gov/reward-for-information-alphv-blackcat-ransomware-as-a-service/)
- [ALPHV-BlackCat ransomware group goes dark | Barracuda](https://blog.barracuda.com/2024/03/06/alphv-blackcat-ransomware-goes-dark)
- [BlackCat (cyber gang) - Wikipedia](https://en.wikipedia.org/wiki/BlackCat_(cyber_gang))
- [BlackCat Ransomware: Analysis and Detection | SentinelOne](https://www.sentinelone.com/anthology/blackcat/)
- [Justice Department Disrupts ALPHV/Blackcat | DOJ](https://www.justice.gov/archives/opa/pr/justice-department-disrupts-prolific-alphvblackcat-ransomware-variant)
- [ALPHV BlackCat Ransomware: Technical Deep Dive | Trustwave](https://www.trustwave.com/en-us/resources/blogs/trustwave-blog/alphv-blackcat-ransomware-a-technical-deep-dive-and-mitigation-strategies/)