---
title: 'Javascript - Obfuscation 1'
description: 'Déobfuscation de code JavaScript pour révéler un mot de passe caché'
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 5. Javascript - Obfuscation 1

**Objectif :** Trouver mot de passe du site  
**Méthode :** Analyse code source de la page + déobfuscation du code js de login  
**Outils utilisés :** Code source de la page  
**Temps :** 5 minutes  
**Flag :** `cpasbiendurpassword`

### Solution

Le code JavaScript est obfusqué mais peut être déobfusqué manuellement pour révéler le mot de passe.

![Challenge JavaScript Obfuscation](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.43.09.png)

**Étapes :**
1. Examiner le code source de la page
2. Localiser le code JavaScript obfusqué contenant la logique de login
3. Déobfusquer le code (décryptage de chaînes, décodage)
4. Extraire le mot de passe en clair

![Analyse du code obfusqué](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.47.09.png)

![Déobfuscation du code](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.47.18.png)
