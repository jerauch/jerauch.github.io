---
layout: post
title: Migrer une base MySQL vers une base Azure SQL Database
published: true
---

Dans le cadre d'un projet nous avons dû migrer une base MySQL vers une base "SQL Database" hébergée chez Azure. Microsoft propose un outil de migration, voilà la procédure à suivre.

Pré-requis :

- Il faut avoir un accès vers la base MySQL (nom du serveur, nom de la base, login et mot de passe)
- Il faut créer le serveur Azure SQL ainsi qu'une base de données. Lors de la création de la base il faudra noter son nom, ainsi que le login et le mot de passe permettant d'accéder à la base. 
- Il faut aussi autoriser votre adresse IP à accéder à la base Azure SQL Database en utilisant le bouton "Set server Firewall" :

![]({{site.baseurl}}/https://github.com/jerauch/jerauch.github.io/blob/master/_posts/SQL1.png?raw=true)

- Installer la dernière version de l'outil de migration : [https://www.microsoft.com/download/confirmation.aspx?id=54257](https://www.microsoft.com/download/confirmation.aspx?id=54257)

- Installer le driver ODBC MySQL

La procédure :

- Commencez par installer l'outil de migration. 

- Créer un nouveau projet de type migration vers ...

- Se connecter à la base MySQL avec le bouton ...

- Se connecter à la base Azure avec le bouton. Pour l'authentification, il faut utiliser le mode ... avec le login / mot de passe définit à la création de la base.

- La partie haute de l'écran présente la base MySQL et la partie basse la base Azure. Dans MySQL, aller sur le dossier "Tables" et faire clic droit puis " ". _Ceci va uniquement préparer la création de la structure des tables dans Azure, les tables seront créées à l'étape suivante!_

- Ensuite il faut aller dans l'écran Azure, sur les tables et faire "...". Ceci permet de créer les tables dans Azure.

- Et on termine en cliquant droit sur les tables dans MySQL puis ...

Selon la volumétrie la durée de transfert peut être plus ou moins longue. 
