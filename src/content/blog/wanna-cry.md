---
title: "WannaCry (2017) - L'attaque ransomware qui a paralysé le monde"
description: "Analyse complète de l'attaque WannaCry : vulnérabilité EternalBlue, propagation mondiale et impact de 200 000 systèmes infectés"
pubDate: "Jul 2 2025"
heroImage: "https://home.cern/sites/default/files/2018-06/image001.png"
---

## Quelle est la vulnérabilité exploitée ?

WannaCry a exploité la vulnérabilité **CVE-2017-0144** (EternalBlue), une faille dans le protocole SMB (Server Message Block) de Microsoft Windows . Cette vulnérabilité permettait l'exécution de code à distance sur des systèmes Windows non patchés .

## Comment l'attaque s'est-elle déroulée ?

L'attaque a débuté le 12 mai 2017 et s'est propagée rapidement à travers le monde  :

1. **Exploitation** : Les attaquants ont utilisé l'exploit EternalBlue, développé par la NSA et divulgué par le groupe Shadow Brokers 
2. **Propagation** : Le ransomware se propageait automatiquement sur les réseaux via la vulnérabilité SMB 
3. **Chiffrement** : Une fois installé, WannaCry chiffrait les fichiers et demandait une rançon de .1781 bitcoins, environ 300$ US 
4. **Kill switch** : Marcus Hutchins a découvert un domaine de contrôle qui a permis de stopper la propagation 

## Qui a été touché ?

- Plus de **200 000 systèmes** dans plus de 150 pays 
- **NHS britannique** : hôpitaux forcés de rediriger des ambulances 
- **Grandes entreprises** : FedEx, Honda, Nissan 
- **Infrastructure critique** : systèmes de transport, énergétiques
- **Organisations gouvernementales** dans le monde entier

## Quels ont été les impacts ?

- **Interruption des services médicaux** : opérations annulées, systèmes d'imagerie hors service 
- **Paralysie des transports** : retards dans les livraisons, perturbations logistiques
- **Pertes économiques** : estimées à plusieurs milliards de dollars
- **Panique mondiale** : première attaque ransomware de cette ampleur

## Quel coût estimé ?

- **Petite entreprise** : 50 000 € à 200 000 € (downtime, récupération, expertise)
- **Moyenne entreprise** : 500 000 € à 2 000 000 € (systèmes multiples, perte de données)
- **Grande entreprise** : 5 000 000 € à 50 000 000 € (infrastructure complexe, impact global)

## Comment s'en protéger ?

1. **Mise à jour systématique** : Appliquer le patch MS17-010 et maintenir les systèmes à jour 
2. **Segmentation réseau** : Isoler les systèmes critiques
3. **Filtrage email** : Bloquer les pièces jointes suspectes avec des filtres anti-spam robustes 
4. **Sauvegardes régulières** : Sauvegardes hors ligne et testées
5. **Surveillance réseau** : Détecter les communications anormales
6. **Formation utilisateurs** : Sensibilisation aux menaces

## Pourquoi est-ce difficile à éviter ?

- **Systèmes legacy** : Nombreux systèmes anciens difficiles à mettre à jour 
- **Propagation automatique** : Aucune action utilisateur requise 
- **Vitesse de propagation** : Infection en quelques heures
- **Complexité des infrastructures** : Difficile de patcher tous les systèmes rapidement 
- **Exploit gouvernemental** : Utilisation d'outils développés par les services de renseignement

## Dans le contexte de votre entreprise, que feriez-vous ?

1. **Audit de sécurité immédiat** : Inventaire de tous les systèmes Windows et vérification des patchs
2. **Plan de continuité** : Développement de procédures de fonctionnement en mode dégradé
3. **Stratégie de sauvegarde renforcée** : Sauvegardes automatisées et déconnectées
4. **Formation du personnel** : Sensibilisation aux ransomwares et procédures d'urgence
5. **Surveillance 24/7** : Mise en place d'un SOC pour détecter les anomalies
6. **Tests réguliers** : Simulations d'attaques et tests de récupération

## Sources

- [WannaCry ransomware attack - Wikipedia](https://en.wikipedia.org/wiki/WannaCry_ransomware_attack)
- [CVE-2017-0143 Windows SMB RCE Vulnerability (WannaCry) – Kaseya](https://helpdesk.kaseya.com/hc/en-gb/articles/4407526903953-CVE-2017-0143-Windows-SMB-RCE-Vulnerability-WannaCry)
- [What was the WannaCry ransomware attack? | Cloudflare](https://www.cloudflare.com/learning/security/ransomware/wannacry-ransomware/)
- [Ransomware WannaCry: All you need to know | Kaspersky](https://www.kaspersky.com/resource-center/threats/ransomware-wannacry)
- [WannaCry Ransomware Vulnerability in Windows Servers | Trend Micro](https://helpcenter.trendmicro.com/en-us/article/tmka-19803)
- [Indicators Associated With WannaCry Ransomware | CISA](https://www.cisa.gov/news-events/alerts/2017/05/12/indicators-associated-wannacry-ransomware)