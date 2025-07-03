---
title: 'Javascript - Obfuscation 3 (Bonus)'
description: 'Déobfuscation avancée avec console.log et String.fromCharCode'
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## Bonus : Javascript - Obfuscation 3

**Objectif :** Trouver le flag dans du code JavaScript obfusqué  
**Méthode :** Console.log + String.fromCharCode pour déobfuscation  
**Outils utilisés :** Console Chrome / Sources  
**Temps :** 5 minutes  
**Flag :** `786OsErtk12`

### Solution

Déobfuscation d'un code JavaScript avec technique de logging et conversion de caractères.

![Challenge JavaScript Obfuscation 3](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.06.23.png)

**Étapes :**
1. Ouvrir la console et aller dans Sources
2. Identifier le code obfusqué qui tente de brouiller les pistes
3. Ajouter un `console.log()` à la dernière ligne de la fonction pour afficher la chaîne
4. Utiliser `String.fromCharCode()` avec le résultat précédent
5. Obtenir le flag déobfusqué

![Analyse du code obfusqué](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.06.30.png)

![Déobfuscation avec console.log](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.06.38.png)

![Flag révélé](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.06.53.png)
