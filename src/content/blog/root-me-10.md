---
title: 'AST - Deobfuscation'
description: "Déobfuscation d'un Abstract Syntax Tree pour récupérer un flag"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme11-0.png'
---

## 10. AST - Deobfuscation

**Objectif :** Déobfusquer un AST (Abstract Syntax Tree) pour trouver le flag  
**Méthode :** Analyser AST -> identifier la fonction gen_sensor -> traduire en code  
**Outils utilisés :** Code (dans console inspecteur)  
**Temps :** 25 minutes  


### Solution

Analyse et déobfuscation d'un Abstract Syntax Tree pour récupérer une fonction génératrice.

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme11-0.png"/></div>

**Étapes :**
1. Analyser la structure AST
2. Identifier la fonction `gen_sensor()` dans l'arbre
3. Reconstruire le code JavaScript à partir de l'AST
4. Exécuter `gen_sensor()` dans la console
5. Obtenir le flag généré par la fonction

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme11-1.png"/></div>

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme11-2.png"/></div>
