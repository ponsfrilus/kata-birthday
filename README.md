# Kata : Anniversaire

<!-- start:apropos -->
> **À propos**
>
> ⓘ Ceci est la donnée d'un [kata], un _exercice de programmation_ qui se
> déroule généralement dans le cadre d'un [coding dojo]. Il est proposé aux
> membres du dojo de l'[EPFL] et fait partie d'une collection de différents
> katas identifiés par le tag **[epfl-dojo-kata]** sur GitHub.  
> Vous êtes plus que bienvenu·e d'essayer de le réaliser dans le langage de
> programmation de votre choix. Lorsque c'est terminé, ajoutez-vous à la liste
> de ceux qui l'ont fait dans ce document en proposant une [Pull Request]. Vous
> pouvez également partager votre intérêt pour ce dépôt en
> le «[stargazant]», c'est à dire en lui ajoutant une ⭐.  
> Bonne lecture et bon code !

[kata]: https://fr.wikipedia.org/wiki/Coding_dojo#Kata
[coding dojo]: https://fr.wikipedia.org/wiki/Coding_dojo
[EPFL]: https://www.epfl.ch
[epfl-dojo-kata]: https://github.com/topics/epfl-dojo-kata
[Pull Request]: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests
[stargazant]: https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars
<!-- end:apropos -->

## But

Le but de ce kata est d'implémenter, dans le langage de programmation de votre
choix, un programme qui envoie des mails de rappel d'anniversaire.

Le programme a une liste composée des informations suivantes :
  - Prénom Nom
  - Date de naissance (au format [ISO-8601])
  - Email

Lorsque le script est appellé, il effectue les actions suivantes :
  1. Vérifie si c'est l'anniversaire d'une personne de la liste ;
  2. Pour chaque personne dont c'est l'anniversaire, envoie un mail de rappel
     à toutes les autres personnes.

Le contenu du mail est laissé à charge du lecteur, mais voici une proposition
pour les plus indécis d'entre vous :

> Titre : C'est l'anniverssaire de John Doe !  
>
> Pssst,  
>
> C'est l'anniverssaire de John Doe aujourd'hui ! Il a 22 ans.  
> Tu peux lui envoyer un email à John Doe <john.doe@example.com>.
>
> A+  
> KataBirthday


## Objectifs

* Entraîner la programmation (structure de donnée, boucles, etc.)
* Entraîner des tâches de _sysadmin_ :
  * appels de script quotidiennement à une heure donnée ([cron])
  * envois de mails ([sendmail], [MTA])


## Je l'ai fait 💪

* La version d'[@Azecko](https://github.com/Azecko) a été faite en `NodeJS` et
  est disponible [ici](https://github.com/Azecko/kata-birthday).
* La version de [@octocat](https://github.com/octocat) a été faite en `langage`
  et est disponible [ici](https://#).


## Pour aller plus loin

Voici quelques idées pour faire évoluer le projet :
* Ajouter une citation aléatoire dans le message ;
* Ajouter une image / gif aléatoire dans le message (`cid:`);
* Créer une interface de gestion des utilisateurs ;
* Ajouter la possibilité de recevoir les messages par messagerie instantanée,
  par exemple Discord ou Telegram ;
* Envoyer les mails au format text et HTML ([MIME multipart](https://en.wikipedia.org/wiki/MIME#Multipart_messages));
* etc...

[ISO-8601]: https://fr.wikipedia.org/wiki/ISO_8601
[cron]: https://fr.wikipedia.org/wiki/cron
[sendmail]: https://fr.wikipedia.org/wiki/sendmail
[MTA]: https://fr.wikipedia.org/wiki/Mail_Transfer_Agent
