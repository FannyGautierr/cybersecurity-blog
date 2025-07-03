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

![Challenge JavaScript Native Code](/src/assets/root_me/rootme7-0.png)

**Étapes :**
1. Examiner le code source
2. Identifier la fonction de login
3. Utiliser `.toString()` dans la console pour afficher le contenu de la fonction
4. Analyser la fonction décompilée pour extraire le mot de passe

![Challenge JavaScript Native Code](/src/assets/root_me/rootme7-2.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme7-3.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme7-4.png)