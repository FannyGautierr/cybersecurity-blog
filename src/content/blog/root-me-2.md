---
title: 'Javascript - Authentification'
description: "Contournement d'authentification JavaScript : analyse du code source pour bypasser la sécurité"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 2. Javascript - Authentification

**Objectif :** Bypass l'authentification du site  
**Méthode :** Analyse code source du site -> login.js  
**Outils utilisés :** Inspecteur Chrome / Fichier sources  
**Temps :** 2 minutes  
**Flag :** `sh.org`

### Solution

L'authentification est implémentée côté client, permettant de découvrir les identifiants en analysant le code JavaScript.

![Challenge JavaScript Authentification](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.24.06.png)

**Étapes :**
1. Ouvrir les DevTools Chrome
2. Aller dans l'onglet "Sources"
3. Examiner le fichier `login.js`
4. Analyser la logique d'authentification pour trouver les identifiants hardcodés
5. Utiliser ces identifiants pour se connecter

![Analyse du code source JavaScript](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.24.20.png)

![Solution JavaScript Authentification](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.24.30.png)
