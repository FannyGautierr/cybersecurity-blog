---
title: 'Javascript - Native Code'
description: 'Analyse de fonctions JavaScript natives pour révéler des secrets'
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme7-0.png'
---

## 7. Javascript - Native Code

**Objectif :** Trouver le mot de passe du site  
**Méthode :** Analyse code source + utilisation de la console pour toString() code -> obtenir la fonction de login -> donc le mot de passe  
**Outils utilisés :** Code source de la page / Console chrome  
**Temps :** 5 minutes  


### Solution

Le mot de passe est caché dans une fonction JavaScript native qu'il faut analyser.

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme7-0.png"/></div>

**Étapes :**
1. Examiner le code source
2. Identifier la fonction de login
3. Utiliser `.toString()` dans la console pour afficher le contenu de la fonction
4. Analyser la fonction décompilée pour extraire le mot de passe

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme7-2.png"/></div>
<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme7-3.png"/></div>
<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme7-4.png"/></div>