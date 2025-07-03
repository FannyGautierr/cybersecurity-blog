---
title: 'Javascript - Source'
description: "Analyse du code source JavaScript pour découvrir des informations d'authentification"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 3. Javascript - Source

**Objectif :** Bypass l'authentification du site  
**Méthode :** Analyse code source du site -> web-client/ch1  
**Outils utilisés :** Inspecteur Chrome / Fichier sources  
**Temps :** 2 minutes  
**Flag :** `123456azerty`

### Solution

Similar au précédent, ce challenge nécessite d'analyser le code source JavaScript pour découvrir des informations d'authentification.

![Challenge JavaScript Source](/src/assets/root_me/rootme3-0.png)

**Étapes :**
1. Accéder aux sources via les DevTools
2. Naviguer vers `web-client/ch1`
3. Examiner le code pour identifier la logique d'authentification
4. Extraire les identifiants ou la méthode de bypass

