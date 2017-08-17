# Traduire WordPress, ses thèmes & extensions

Ce guide a pour objectif d’aider les personnes souhaitant participer à la traduction de WordPress et de son écosystème à comprendre comment fonctionne le système **translate.wordpresss.org**.

## L’internationalisation de WordPress et de son écosystème

WordPress est traduit dans plus de 150 langues par des bénévoles de la communauté mondiale, regroupés en équipe de polyglottes. 
Chacun peut contribuer à son développement en participant à la traduction française :

- du cœur du CMS
- de ses extensions
- de ses thèmes
- au niveau « meta » : documentation, wp.org, apps, etc.

# Le WordPress Translation Day

- Un évènement annuel mondial
- Stats 2016 : **780 traducteurs** dans **133 langues** ont produit **60426 traductions** lors de **67 évènements** dans le monde !

En 2017, la troisième édition :
- Un évènement **sur 24h** dans le monde entier et tous les fuseaux horaires
- Des dizaines d’évènements locaux
- Des conférences diffusées en streaming toute la journée
- Un hashtag : **#WPTranslationDay**

Site officiel → https://wptranslationday.org 

# Structuration de la communauté

## General Translation Editor (GTE)

- Responsable de la traduction pour une localisation (exemple : *fr_FR*)
- Réalise et valide les traductions proposées sur tous les projets d’une localisation
- Valide les demandes de nouveaux PTE et guide la communauté

## Project Translation Editor (PTE)

- Responsable d’un projet (thème, extension) pour une localisation
- Réalise et valide les traductions proposées sur le projet dont il est responsable pour une localisation

## Personne disposant d’un compte wordpress.org

- Peut proposer des traductions pour validation par un GTE ou par un PTE

# La diffusion des traductions réalisées : le système *Translate*

Une fois la traduction validée par un PTE ou par un GTE, et lorsque le projet (WordPress, thème, extension) est validé à 95% ou plus dans une localisation donnée, le système *Translate* : 

- construit un **paquet de langue**
- **notifie** les utilisateurs de WordPress via leur administration pour qu’ils puissent mettre à jour la traduction du projet depuis leur interface d’administration

# Gestion des traductions sur votre serveur

Les fichiers de traduction sont situées sur wp-content/languages

Dans ce répertoire, on trouve les traductions du cœur de WordPress.

Les traductions des thèmes et extensions sont situées dans les sous-dossiers */themes* et */plugins*

