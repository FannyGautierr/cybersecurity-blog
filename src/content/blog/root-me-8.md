---
title: 'Javascript - Webpack'
description: 'Décompilation de bundles Webpack pour extraire des flags cachés'
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 8. Javascript - Webpack

**Objectif :** Trouver le flag  
**Méthode :** Code source -> recherche Google -> décompilation avec outil en ligne  
**Outils utilisés :** Code sources / Devtools / Google Search  
**Temps :** 15 minutes  
**Flag :** `BecauseSourceMapsAreGreatForDebuggingButNotForProduction`

### Solution

Ce challenge implique l'analyse d'un bundle Webpack pour extraire le flag.

![Challenge JavaScript Webpack](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.55.39.png)

**Étapes :**
1. Analyser le code source pour identifier le bundle Webpack
2. Copier le code obfusqué
3. Utiliser un décompilateur en ligne (https://onecompiler.com/javascript/3zn4nw69x)
4. Rechercher "flag" dans le code décompilé (Cmd+F)
5. Localiser le flag dans le code déobfusqué

![Code Webpack obfusqué](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.56.02.png)

![Décompilation et recherche du flag](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.56.09.png)

![Flag trouvé dans le code décompilé](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.57.54.png)
