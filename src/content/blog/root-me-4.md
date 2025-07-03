---
title: 'Javascript - Authentification 2'
description: "Deuxième challenge d'authentification JavaScript avec une approche différente"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme4-0.png'
---

## 4. Javascript - Authentification 2

**Objectif :** Bypass l'authentification du site  
**Méthode :** Analyse code source du site -> login.js  
**Outils utilisés :** Inspecteur Chrome / fichiers Sources  
**Temps :** 2 minutes  


### Solution

Une autre variante d'authentification côté client vulnérable.

![Challenge JavaScript Authentification 2](/src/assets/root_me/rootme4-0.png)

**Étapes :**
1. Analyser le fichier `login.js` dans les sources
2. Identifier la logique de vérification des identifiants
3. Découvrir les credentials cachés dans le code
4. Utiliser ces informations pour contourner l'authentification

![Challenge JavaScript Authentification 2](/src/assets/root_me/rootme4-1.png)

![Challenge JavaScript Authentification 2](/src/assets/root_me/rootme4-2.png)
