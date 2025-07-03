---
title: 'Javascript - Obfuscation 2'
description: "Déobfuscation avancée avec plusieurs couches d'encodage"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---
## 6. Javascript - Obfuscation 2

**Objectif :** Trouver mot de passe du site  
**Méthode :** Analyse code source + utilisation de la console pour unescape le mot de passe (deux fois + String.fromCharCode)  
**Outils utilisés :** Code source de la page / Console chrome  
**Temps :** 5 minutes  
**Flag :** `hDufjdki156`

### Solution

Le mot de passe est obfusqué avec plusieurs couches d'encodage nécessitant l'utilisation de la console JavaScript.

![Challenge JavaScript Obfuscation 2](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.49.15.png)

**Étapes :**
1. Analyser le code source pour identifier les chaînes obfusquées
2. Ouvrir la console Chrome
3. Utiliser `unescape()` pour décoder le premier niveau
4. Appliquer `String.fromCharCode()` pour le décodage final
5. Obtenir le mot de passe déobfusqué

![Déobfuscation avec la console](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.51.35.png)

![Solution trouvée](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.51.48.png)
