## Introduction

* Contexte
* Problématique
* Use case 
* Scénarios d’attribut de qualité
* Vues de structures architecturales

Mailtrust est une entreprise axée sur le service à la clientèle. Il est extrêmement important que les techniciens de l'assistance    technique puissent examiner les journaux de messagerie afin de résoudre les problèmes des clients.

## Logging V1.0 ##

* Contexte:
Les logs sont stockés dans des fichiers texte sur le disque local de chaque serveur de messagerie et sont conservés pendant 14 jours. Les techniciens de support n’ont pas accès au serveur et doivent créer un ticket auxingenieurs pour que ces derniers leurs transmettent.
* Problématique
Si l'on depasse une douzaine de serveurs, ce processus manuel de connexion à chaque serveur prend trop de temps aux ingénieurs. (perte d'éfficacité)
* Use case
En tant que technicien de support je veux pouvoir accéder aux logs efficacement afin de traiter la demande client.
* Discussion (contexte)
* Attributs qualités
Efficacité
* Structures architecturales

