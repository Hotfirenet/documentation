---
layout: default
title: Documentation
description: Les flotteurs de la gamme Ico conçus par la société Ondilo sont des capteurs Wifi qui permettent l'analyse de votre piscine ou de votre SPA.
parent: Ondilo
grand_parent: Jeedom
nav_order: 1
---

# Grocy
{: .no_toc }

## Sommaire
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Installation du plugin Ondilo - ICO

L'installation du plugin se fait depuis l'interface gestion des plugins et / ou depuis le market.

---

## Configuration du plugian Ondilo - ICO

Dans un premier temps vous devez vous authentifier à votre compte Ondilo depuis la page de configuration.

{% include lightbox.html src="jeedom/plugin-ondilo/images/authentification-a-api-ondilo.png" data="ondilo" title="Authentification à l'api Ondilo" imgstyle="width:100%;display: block;margin: 0 auto;" %}

Une nouvelle page va s'ouvrir, vous devez renseigner vos identifiants. (Pas de craintes vous êtes sur le site d'ondilo le fabriquant de l'ICO. Le plugin ne sauvegarde aucun ni login, ni mot de passe).

**ATTENTION** le choix de la langue est important, car les recommandations seront dans la langue sélectionnée.

{% include lightbox.html src="jeedom/plugin-ondilo/images/authentification-ondilo.png" data="ondilo" title="Authentification à l'api Ondilo" imgstyle="width:100%;display: block;margin: 0 auto;" %}

Une fois connecté, vous revenez sur une page blanche. Vous pouvez fermer celle-ci et recharger votre page de configuration.

### Custom Widget

Vous pouvez choisir d'utiliser la tuile personnalisé ou les widgets natifs à jeedom. A vous de choisir en cochant cette option.

{% include lightbox.html src="jeedom/plugin-ondilo/images/activer-widget-custom.png" data="ondilo" title="Activation widget personnalisé" imgstyle="width:100%;display: block;margin: 0 auto;" %}

Ce qui donnera:

> Widget Natif

{% include lightbox.html src="jeedom/plugin-ondilo/images/standard-ondilo-widget-jeedom.png" data="ondilo" title="Widget Natif" imgstyle="width:100%;display: block;margin: 0 auto;" %}

> Widget (Tuile) personnalisé

{% include lightbox.html src="jeedom/plugin-ondilo/images/custom-ondilo-widget-jeedom.png" data="ondilo" title="Widget Natif" imgstyle="width:100%;display: block;margin: 0 auto;" %}

### Activation des recommandations

Il est possible de ne pas récupérer les recommandations proposées par Ondilo en ne cochant pas cette option.

{% include lightbox.html src="jeedom/plugin-ondilo/images/ondilo-activer-les-recommandations.png" data="ondilo" title="Activer ou désactiver les recommandations" imgstyle="width:100%;display: block;margin: 0 auto;" %}

---

## Synchronisation de votre Ondilo - ICO

Il est possible d'avoir plusieurs ilots ICO.

{% include lightbox.html src="jeedom/plugin-ondilo/images/synchronisation-jeedom-ondilo-ico.png" data="ondilo" title="Synchronisation des ilots" imgstyle="width:100%;display: block;margin: 0 auto;" %}

### Les équipements

Pour savoir ce qu'est un équipement je vous invites à lire les [Concepts Jeedom sur les équipements](https://doc.jeedom.com/fr_FR/concept/#tocAnchor-3)

#### Un ilot ICO
Un îlot ICO est un équipement dans Jeedom, ainsi, il dispose de commande type informations ou actions. Voici la liste des commandes:

- (info) Température
- (info) Acidité (pH)
- (info) Désinfection (ORP)
- (info) Sel si piscine au sel
- (info) Conductivité (TDS)
- (info) Puissance du signal WIFI (%)
- (info) Vu Dernière Fois
- (action) Rafraichir 

Un équipement dispose d'un paramètre permettant d'indiquer le niveau de batterie. Vous pouvez retrouver l'info sur le widget ou dans la partie: Analyse > Equipements : exemple [https://jeedom.local/index.php?v=d&p=eqAnalyse](https://jeedom.local/index.php?v=d&p=eqAnalyse)

{% include lightbox.html src="jeedom/plugin-ondilo/images/ondilo-battery.png" data="ondilo" title="Analyse des équipements, niveau de batterie" imgstyle="width:100%;display: block;margin: 0 auto;" %}

#### Les recommandations

Les recommandations sont visibles dans le centre de message:

{% include lightbox.html src="jeedom/plugin-ondilo/images/centre-de-message-jeedom-recommandations-ondilo.png" data="ondilo" title="Synchronisation des ilots" imgstyle="width:100%;display: block;margin: 0 auto;" %}

Pour le moment les recommandations proposées par l'api de Ondilo se résume au type **Waiting**, c'est à dire celles qui demandent une validations de votre part.

---

## FAQ

Est ce que le plugin utlise des API tierces ?

Oui le plugin utilise l'[api officielle de Ondilo](https://interop.ondilo.com/docs/api/customer/v1/).

---

## Remerciements