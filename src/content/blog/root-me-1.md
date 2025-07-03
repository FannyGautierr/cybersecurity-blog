---
title: 'HTML - Boutons Désactivés'
description: 'Bypass de sécurité côté client : activer un bouton désactivé pour accéder à une fonction cachée'
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme1.png'
---

## 1. HTML - Boutons Désactivés

**Objectif :** Activer un bouton désactivé pour accéder à une fonction cachée  
**Méthode :** Modification DOM - Suppression attribut disabled  
**Outils utilisés :** Inspecteur Chrome  
**Temps :** 2 minutes  


### Solution

Ce challenge consiste à bypasser une restriction côté client en modifiant le DOM. Un bouton est désactivé via l'attribut HTML `disabled`, empêchant l'utilisateur de cliquer dessus normalement.

![Challenge Root-Me HTML Boutons Désactivés](/src/assets/root_me/rootme1.png)

**Étapes :**
1. Ouvrir l'inspecteur Chrome (F12)
2. Localiser l'élément `<button>` avec l'attribut `disabled`
3. Supprimer l'attribut `disabled` en modifiant le HTML
4. Le bouton devient alors cliquable et révèle la fonction cachée

![Solution HTML Boutons Désactivés](/src/assets/root_me/root-me1-2.png)

Cette technique illustre pourquoi la sécurité ne doit jamais reposer uniquement sur des contrôles côté client.
