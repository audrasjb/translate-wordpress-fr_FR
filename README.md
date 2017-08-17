# Traduire WordPress, ses thèmes & extensions

![Logo WordPress Translation Day 2017](/images/translate_wptd2017.png)

Ce guide a été réalisé dans le cadre de la préparation du WordPress Translation Day 2017, au départ pour le meetup local WP Drôme-Ardèche, puis proposé à tous les organisateurs de meetups locaux francophones.

Il a pour objectif d’aider les personnes souhaitant participer à la traduction de WordPress et de son écosystème à comprendre comment fonctionne le système **translate.wordpresss.org**.

## L’internationalisation de WordPress et de son écosystème

WordPress est traduit dans plus de 150 langues par des bénévoles de la communauté mondiale, regroupés en équipe de polyglottes. 
Chacun peut contribuer à son développement en participant à la traduction française :

- du cœur du CMS
- de ses extensions
- de ses thèmes
- au niveau « meta » : documentation, wp.org, apps, etc.

## Le WordPress Translation Day

- Un évènement annuel mondial
- Stats 2016 : **780 traducteurs** dans **133 langues** ont produit **60426 traductions** lors de **67 évènements** dans le monde !

En 2017, la troisième édition :
- Un évènement **sur 24h** dans le monde entier et tous les fuseaux horaires
- Des dizaines d’évènements locaux
- Des conférences diffusées en streaming toute la journée
- Un hashtag : **#WPTranslationDay**

Site officiel → https://wptranslationday.org 

## Structuration de la communauté

### General Translation Editor (GTE)

- Responsable de la traduction pour une localisation (exemple : *fr_FR*)
- Réalise et valide les traductions proposées sur tous les projets d’une localisation
- Valide les demandes de nouveaux PTE et guide la communauté

### Project Translation Editor (PTE)

- Responsable d’un projet (thème, extension) pour une localisation
- Réalise et valide les traductions proposées sur le projet dont il est responsable pour une localisation

### Personne disposant d’un compte wordpress.org

- Peut proposer des traductions pour validation par un GTE ou par un PTE

## La diffusion des traductions réalisées : le système *Translate*

Une fois la traduction validée par un PTE ou par un GTE, et lorsque le projet (WordPress, thème, extension) est validé à 95% ou plus dans une localisation donnée, le système *Translate* : 

- construit un **paquet de langue**
- **notifie** les utilisateurs de WordPress via leur administration pour qu’ils puissent mettre à jour la traduction du projet depuis leur interface d’administration

## Gestion des traductions sur votre serveur

Les fichiers de traduction sont situées sur wp-content/languages

Dans ce répertoire, on trouve les traductions du cœur de WordPress.

Les traductions des thèmes et extensions sont situées dans les sous-dossiers */themes* et */plugins*

## Fonctionnement de la traduction : les chaînes de traduction

Une chaîne de traduction est une expression, un mot, une phrase, découpée et isolée et utilisant la syntaxe standard et internationale fournie par PHP : **gettext**

Exemple :

`__(‘Hello word’, ‘textdomain’)`

- Le premier paramètre, ici « Hello word » est l’élément traduisible.
- Le second paramètre, ici « textdomain » permet d’identifier le projet auquel la chaîne appartient.

## Comment devenir traducteur

1. Connectez-vous à WordPress.org ou créez un compte.
2. Visitez la page des projets en français sur translate.wordpress.org.
3. Choisissez la localisation à laquelle vous souhaitez contribuer
  - ici : 
French (France)
Français – fr_FR

## Comment traduire

Trouver un projet que vous connaissez/utilisez.

Par exemple ici je clique sur Plugins dans le menu, puis j’utilise le moteur de recherche pour trouver Yoast SEO :

### La page de traduction d’un projet

(image)

### Les statuts des chaînes de traduction

- **translated**/**approved** : traduction validée
- **untranslated** : pas encore de traduction proposée
- **waiting** : une traduction a été proposée mais n’a pas encore été validée
- **fuzzy** : traduction enregistrée en brouillon, doit être validée manuellement

### Traduire une chaîne avec Translate

Ci-dessous, la chaîne « Remind me again in 4 weeks » n’est pas traduite. Je double-clique dans la cellule correspondante de la colonne « Translation » (ou sur « Details »).

(image)

Traduire la chaîne, puis cliquer sur « Suggest new translation » :

(image)

La chaîne apparaît maintenant en **orange**, elle est en attente de validation :

(image)

On peut encore la modifier en cliquant sur « Details » :

(image)

### À partir du moment où une chaîne proposée a été validée…

Une fois une chaîne validée par un PTE ou un GTE : 
- Celle-ci apparaîtra avec le statut `translated` dans le pack de langues du projet (en vert)
- Elle sera déployée sur toutes les installations utilisant ce projet (thème ou extension)
- Vous serez reconnu comme un contributeur officiel du projet WordPress ! 

(ง'̀-'́)ง

### Que faire pour demander la validation de vos traductions ?

Plutôt que d’attendre qu’un GTE ou PTE passe par là, le plus simple est de demander la validation de vos chaînes directement : 
- S’inscrire sur le Slack WordPress-fr → https://wpfr.net/slack/ 
- Aller dans le channel #traductions et poster un lien vers le projet que vous avez traduit

Vous pouvez en profiter pour y poser vos questions éventuelles : la communauté est là pour vous répondre 😊

## Recommandations générales

- Suivre le [glossaire du cœur de WordPress](https://translate.wordpress.org/projects/wp/dev/fr/default/glossary), il constitue la ligne directrice de la traduction de WordPress.
- Privilégier un langage formel. Le « vous » plutôt que le « tu ».
- La traduction doit être facile à lire et à comprendre, même pour les utilisateurs qui n’ont pas de bagage technique spécifique.
- Utiliser des phrases courtes et claires. Éviter la voix passive et les phrases trop longues.
- Le ton doit refléter celui du texte original.
- Ne pas traduire littéralement.
- Ne pas traduire le nom des thèmes, extensions.

### Suivre les règles typographiques françaises

Gestion de la ponctuation et des espaces insécables
→ saisir ALT+255 sur Windows et ALT+SPACE sur MacOS pour produire un espace insécable

Utiliser les guillemets français `…`
→ saisir ALT+0171 et ALT+0187 sur Windows ou ALT+7 et ALT+SHIFT+7 sur MacOS

Utiliser l’apostrophe courbe française `’` au lieu du guillemet droit `'`
→ saisir ALT+0146 sur Windows ou ALT+SHIFT+4 sur MacOS

Règles typographiques de base : https://fr.wordpress.org/2016/04/22/regles-typographiques-de-base/ 

## Devenir Project Translation Editor (PTE)

- Vous êtes éditeur de thèmes ou d’extensions ?
- Vous êtes un utilisateur assidu d’un thème ou d’une extension qui ne dispose pas de PTE en fr_FR ?
- Vous avez déjà l’expérience d’avoir traduit plusieurs chaînes de caractères validées par la communauté ?

Dans ce cas, vous pouvez demander à devenir PTE d’un thème ou d’une extension. Vous pourrez alors valider vos propres traductions ainsi que celles proposées par d’autres utilisateurs.

Il suffit d’en faire la demande sur le Slack, channel #traductions.

## Quelques liens pour aller plus loin

- Translate sur WordPress.org 
→ https://translate.wordpress.org
- Le slack WordPress-fr
→ https://wpfr.net/slack/ 
- Le guide de traduction
→ https://fr.wordpress.org/2016/04/22/guide-de-traduction/ 
- Le tableau de cohérence des traductions 
→ https://translate.wordpress.org/consistency 
- Le glossaire anglais-français
→ https://translate.wordpress.org/locale/fr/default/glossary 
- Règles typographiques de base 
→ https://fr.wordpress.org/2016/04/22/regles-typographiques-de-base/ 
- Comment devenir PTE pour un projet fr_FR (en anglais)
→ https://fr.wordpress.org/2015/12/18/how-french-community-handles-pte-requests/ 

## À propos

Ce guide à été réalisé dans le cadre du WP Translation Day 2017.

Crédits : Jb Audras | @audrasjb
Avec les contributions de FX Bénard, Thomas Piron & Pascal Casier

Creative Commons [BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/3.0/fr/)