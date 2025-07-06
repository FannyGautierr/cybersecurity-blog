---
title: 'Javascript - Obfuscation 2'
description: "Déobfuscation avancée avec plusieurs couches d'encodage"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme6-0.png'
---
## 6. Javascript - Obfuscation 2

**Objectif :** Trouver mot de passe du site  
**Méthode :** Analyse code source + utilisation de la console pour unescape le mot de passe (deux fois + String.fromCharCode)  
**Outils utilisés :** Code source de la page / Console chrome  
**Temps :** 5 minutes  


### Solution

Le mot de passe est obfusqué avec plusieurs couches d'encodage nécessitant l'utilisation de la console JavaScript.

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme6-0.png"/></div>

**Étapes :**
1. Analyser le code source pour identifier les chaînes obfusquées
2. Ouvrir la console Chrome
3. Utiliser `unescape()` pour décoder le premier niveau
4. Appliquer `String.fromCharCode()` pour le décodage final
5. Obtenir le mot de passe déobfusqué

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme6-1.png"/></div>

