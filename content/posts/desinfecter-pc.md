---
title: "Guide complet pour nettoyer un PC infecté (2023)"
author: "harvald"
date: 2023-05-02T20:18:04+02:00
draft: false
---

<br/>
<br/>

![PC Portable avec une pop-up de sécurité indiquant la présence d'un malware](/img/malwarebanner.jpg)
<br/>
<br/>

# [Introduction](#introduction)

Vous désirez un guide complet pour nettoyer votre ordinateur ? Je vous ai compilé les meilleures pratiques pour y arriver.

**Sachez tout de même qu'il est parfois difficile de supprimer entièrement un malware récalcitrant et qu'il est toujours mieux de faire une installation propre du système pour être sûr.** 
<br/> Notez que l'outil de réinitialisation Windows ne fait PAS d'installation propre. Il faudra utiliser l'outil [Media Creation Tool](https://www.microsoft.com/fr-fr/software-download/windows10ISO). <br/> <br/>
J'aimerai vous partager quelques ressources qui pourront vous aider à dépanner vos problèmes d'informatiques.\
Elles ont servies d'inspiration pour l'écriture de ce guide.

- [r/TechSupport Wiki](https://rtech.support/docs/safety-security/malware-guide.html) 🇺🇸
- [Awesome Open-Source](https://placeholder.com)



# [Logiciels non-recommandés](#logiciels-non-recommandés)

## Les logiciels de nettoyage
  *CCleaner* et à peu près tout les logiciels de **nettoyage**, **défragmentation**, **optimisation de la RAM** seront juste une surcouche de plus pour votre OS qui gère très bien la ram ainsi que le nettoyage des fichiers temporaires tout seul. <br/>
  >Ces logiciels se lancent souvent au démarrage de votre PC et continuent à tourner en tâche de fond, dans une grande majorité des cas, ils consomment plus de ressources qu'ils n'en font économiser.<br/> <br/>
  > Si vous cherchez à récupérer de l'espace sur votre disque dur, je vous invite à chercher ***"Nettoyage de Disque"*** dans la recherche Windows.

  Les nettoyeurs de registre à la *CCleaner** (encore une fois) finissent souvent par causer plus de dommages que de bien à votre PC. <br/>
  > Je le répète, mais l'OS gère très bien tout ça.

  ## Les Antivirus2
Dans le cadre de la maison, et si vous faites preuve de bon sens, que vous ne téléchargez rien de suspect, que vous n'ouvrez pas de pièces jointes suspectes, que vous utilisez un bloqueur de pub et que votre boîte mail à un anti-spam, vous n'avez pas besoin de plus que Windows Defender, qui est inclus de base avec son système. <br/> <br/>
Etant donné qu'il est developpé par Microsoft, il est bien plus optimisé pour le système que n'importe quel autre antivirus, et il consommera logiquement moins vos précieuses ressources.
> Notez aussi qu'une grosse partie des antivirus (surtout gratuits) sont des [*Bloatwares*](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjNs5P4qNf-AhUwVKQEHZeEBlsQmhN6BAhdEAI&url=https%3A%2F%2Ffr.wikipedia.org%2Fwiki%2FBloatware&usg=AOvVaw1rxAYEV993qfzbAJGcVoCC), les versions gratuites étant la pour que vous payiez un abonnement.

> Si vous souhaitez un complément à Windows Defender, il est conseillé d'utiliser Malwaresbytes en version **gratuite**.<br/>
> Réferez vous à la partie sur les Malwares pour plus d'informations.
  
  ## Les Optimiseurs/Updaters de drivers

Tout les logiciels comme ***Snappy Drivers***, ***DriverBooster***, ou ***DriverEasy*** sont à bannir. Encore une fois, Windows gère très bien les drivers depuis quelques années avec Windows Update. <br/>
>***Point Bonus !*** Les trois logiciels cités ici sont des [PUPs](https://www.malekal.com/adwares-pup-protection/) (Potientially Unwanted Programs)

 Si vos Drivers ne sont pas disponibles sur Windows Update, il est fortement conseillé d'aller sur le ***SITE OFFICIEL*** de l'éditeur du produit et d'y télécharger les Drivers. <br/>
> Vous pourrez facilement les installer avec le ***Gestionnaire de Pérphériques***


# [Adwares](#adwares)

Les adwares ou *logiciels publicitaires* sont des programmes dont la fonction principale est d'afficher des publicités ou des résultats de recherches biaisés pour en tirer profit. \
Ce sont-eux qui remplacent votre moteur de recherche, ou qui installent des *toolbars* pour les plus vieux.

Le logiciel le plus efficace et le plus connu à ma connaissance pour nettoyer ce type d'infections est [AdwCleaner](https://fr.malwarebytes.com/adwcleaner/).

![Interface principale d'Adwcleaner](/img/adwcleaner.png)

## Nettoyer mon navigateur

Après avoir utilisé *Adwcleaner*, il est conseillé de remettre à zéro votre navigateur pour être sûr qu'il ne reste aucun résidu.

****⚠️ Attention ! La remise à zéro du navigateur supprimera votre historique et vos données de navigation ! ⚠️****

- [Réinitialiser Chrome](https://support.google.com/chrome/answer/2765944?hl=fr&co=GENIE.Platform%3DDesktop)
- [Réinitialiser Firefox](https://support.mozilla.org/fr/kb/reparer-firefox-reinitialiser-modules-parametres)
- [Réinitialiser Brave](https://support.brave.com/hc/en-us/articles/360017903152-How-do-I-reset-Brave-settings-to-default-)

# [Malwares](#malwares)

On regroupera ici la majorité des malwares.

- [Rkill](https://www.bleepingcomputer.com/download/rkill/) (Tue les Malwares pour permettre à votre antivirus de se lancer (dans le cas où il aurait été bloqué) et de les nettoyer.)
- [Malwarebytes](https://www.malwarebytes.com) (A utiliser en version gratuite, très bon complément d'Antivirus, peut-être utilisé à côté de Windows Defender)

> En cas d'infection, je vous conseille d'utiliser Rkill puis Malwarebytes ensuite, ça devrait être un bon début.

# [Renforcer ma sécurité](#renforcer-ma-sécurité)

Je le sais, tu le sais, nous le savons, on utilise tous nos mêmes mots de passes. Une solution simple est le **gestionnaire de mots de passe**. <br/>
Quand il s'agit de garder mes mots de passes, je ne fais confiance qu'à l'open-source. Comment faire confiance aux gardien de mes mots de passes si je ne sais pas comment il fonctionne ? <br/>

Il me reste donc à peu près ces gestionnaires :

- [Bitwarden](https://bitwarden.com) (Multi-plateforme, open-source, il est même auto-hébergeable avec [Vaultwarden](https://github.com/dani-garcia/vaultwarden) et Docker pour les petits bidouilleurs)
- [KeePassXC](https://keepassxc.org) (Egalement open-source, multi-plateforme)


