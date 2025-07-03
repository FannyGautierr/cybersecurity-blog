---
title: 'AST - Deobfuscation'
description: "Déobfuscation d'un Abstract Syntax Tree pour récupérer un flag"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 10. AST - Deobfuscation

**Objectif :** Déobfusquer un AST (Abstract Syntax Tree) pour trouver le flag  
**Méthode :** Analyser AST -> identifier la fonction gen_sensor -> traduire en code  
**Outils utilisés :** Code (dans console inspecteur)  
**Temps :** 25 minutes  
**Flag :** `g00d_j0b_easy_deobfuscation`

### Solution

Analyse et déobfuscation d'un Abstract Syntax Tree pour récupérer une fonction génératrice.

![Challenge AST Deobfuscation](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.08.37.png)

**Étapes :**
1. Analyser la structure AST
2. Identifier la fonction `gen_sensor()` dans l'arbre
3. Reconstruire le code JavaScript à partir de l'AST
4. Exécuter `gen_sensor()` dans la console
5. Obtenir le flag généré par la fonction

![Analyse de l'AST](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.09.01.png)

![Exécution de la fonction déobfusquée](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.11.38.png)
