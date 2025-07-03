---
title: 'Javascript - Authentification 2'
description: "Deuxième challenge d'authentification JavaScript avec une approche différente"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 4. Javascript - Authentification 2

**Objectif :** Bypass l'authentification du site  
**Méthode :** Analyse code source du site -> login.js  
**Outils utilisés :** Inspecteur Chrome / fichiers Sources  
**Temps :** 2 minutes  
**Flag :** `HIDDEN`

### Solution

Une autre variante d'authentification côté client vulnérable.

![Challenge JavaScript Authentification 2](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.36.32.png)

**Étapes :**
1. Analyser le fichier `login.js` dans les sources
2. Identifier la logique de vérification des identifiants
3. Découvrir les credentials cachés dans le code
4. Utiliser ces informations pour contourner l'authentification

![Analyse du code d'authentification](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.36.39.png)

![Solution trouvée](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.36.46.png)
