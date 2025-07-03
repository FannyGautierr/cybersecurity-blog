---
title: 'Javascript - Authentification'
description: "Contournement d'authentification JavaScript : analyse du code source pour bypasser la sécurité"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme2-0.png'
---

## 2. Javascript - Authentification

**Objectif :** Bypass l'authentification du site  
**Méthode :** Analyse code source du site -> login.js  
**Outils utilisés :** Inspecteur Chrome / Fichier sources  
**Temps :** 2 minutes  


### Solution

L'authentification est implémentée côté client, permettant de découvrir les identifiants en analysant le code JavaScript.

![Challenge JavaScript Authentification](/src/assets/root_me/rootme2-0.png)

**Étapes :**
1. Ouvrir les DevTools Chrome
2. Aller dans l'onglet "Sources"
3. Examiner le fichier `login.js`
4. Analyser la logique d'authentification pour trouver les identifiants hardcodés
5. Utiliser ces identifiants pour se connecter

![Analyse du code source JavaScript](/src/assets/root_me/rootme2-2.png)

![Solution JavaScript Authentification](/src/assets/root_me/rootme2-3.png)
