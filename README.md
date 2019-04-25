## Introduction

* Contexte
* Problématique
* Use case 
* Scénarios d’attribut de qualité
* Vues de structures architecturales

Mailtrust est une entreprise axée sur le service à la clientèle. Il est important que les techniciens de l'assistance technique puissent examiner les journaux de messagerie afin de résoudre les problèmes des clients.

## Logging V1.0 ##

* Contexte:
Les logs sont stockés dans des fichiers texte sur le disque local de chaque serveur de messagerie et sont conservés pendant 14 jours. Les techniciens de support n’ont pas accès au serveur et doivent créer un ticket aux ingenieurs pour que ces derniers leurs transmettent.
* Problématique:
Si l'on depasse une douzaine de serveurs, ce processus manuel de connexion à chaque serveur prend trop de temps aux ingénieurs. (perte d'éfficacité)
* Use case:
En tant que technicien de support je veux pouvoir accéder aux logs efficacement afin de traiter la demande client.
* Attributs qualités
Efficacité
Maintenabilité
* Structures architecturales:
Voir Logging V1.0.png

## Logging V2.0 ##

* Contexte:
Mise en place d'un outil de recherche de logs que les techniciens du support technique utilisent directement, sans impliquer les ingénieurs. L’équipe de support a reçu un outil Web permettant de rechercher les logs.
Tous les logs sont indexés dans une base de données MySQL
* Problématique:
Au fur et à mesure que les tables grandissent, l'indexation de chaque entrée insérée devient de plus en plus lente. Au cours des premières heures de test, les insertions ont commencé à ralentir et ne pouvaient plus suivre le rythme de réception des données.
* Use case:
En tant que technicien de support je veux pouvoir accéder aux logs efficacement afin de traiter la demande client.
* Attributs qualités
Efficacité
Maintenabilité
Fiablité
* Structures architecturales
Voir Logging V2.0.png

## Logging V3.0 ##

* Contexte:
Implémentation de Apache Hadoop. Hadoop est une implémentation open source de Google File System et de MapReduce, un système spécialement conçu pour le traitement de gros volume de données.
* Problématique:
 Les seuls problèmes rencontrés sont leurs propres bogues.
* Use case:
En tant que technicien de support je veux pouvoir accéder aux logs efficacement afin de traiter la demande client.
* Attributs qualités
Efficacité
Maintenabilité
Fiablité
Stabilité
