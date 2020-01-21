---
layout: post
title: Migrer une base MySQL vers une base Azure SQL Database
published: true
---

Dans le cadre d'un projet nous avons dû migrer une base MySQL vers une base "SQL Database" hébergée chez Azure. Microsoft propose un outil de migration, voilà la procédure à suivre.

Avant de commencer :

- Il faut avoir un accès vers la base MySQL (nom du serveur, nom de la base, login et mot de passe)
- Il faut créer le serveur Azure SQL ainsi qu'une base de données. Lors de la création de la base il faudra noter son nom, ainsi que le login et le mot de passe permettant d'accéder à la base. 
- Il faut aussi autoriser votre adresse IP à accéder à la base Azure SQL Database en utilisant le bouton "Set server Firewall" :

(![SQL1.png]({{site.baseurl}}/_posts/SQL1.png)



