# Politique de confidentialite de yuAs69Bots

*Derniere mise a jour : 15 mai 2026*

## 1. Donnees collectees

yuAs69Bots collecte et stocke uniquement les donnees strictement
necessaires a son fonctionnement, dans une base MongoDB Atlas
chiffree au repos. Aucune donnee ne fait l'objet de tracking
analytique, publicite ou revente.

### Donnees stockees par fonctionnalite

| Fonctionnalite | Donnees stockees |
|---|---|
| Levels (XP) | guild_id, user_id, xp, derniere activite |
| Auto-reponses | guild_id, trigger, reponse, createur |
| Commandes custom | guild_id, nom, reponse, createur |
| Giveaways | guild_id, message_id, prix, gagnants, participants |
| Reaction roles | guild_id, message_id, mapping emoji -> role |
| Rappels | user_id, texte, date programmee |
| Newsletter (pub) | guild_id, user_id (subscribers) |
| Anti-raid / Anti-spam | guild_id, configuration (pas de log des actions) |
| Verification | guild_id, channel_id, role_ids |
| Tickets | guild_id, channel_id (config), threads Discord (par Discord) |
| Tier premium | guild_id, tier, date d'expiration |
| Welcome | guild_id, message de bienvenue, config embed |
| Level-roles | guild_id, niveau, role_id |
| Onboarding | guild_id, questions/choix/roles |
| Codes premium | code, duree, statut, utilisateur final |

Les **identifiants Discord (user_id, guild_id, message_id)** sont des
identifiants publics fournis par Discord. Aucune information personnelle
(vrai nom, email, adresse, telephone, IP, mot de passe) n'est jamais
collectee.

## 2. Donnees NON collectees

yuAs69Bots ne collecte JAMAIS :
- Le contenu des messages prives (DMs) entre utilisateurs
- Le contenu des messages dans les salons (hors triggers explicites
  comme auto-reponses ou commandes prefixees `?nom`)
- Les mots de passe, emails, adresses IP, numeros de telephone
- Les habitudes de navigation, donnees de tracking, cookies
- Toute donnee a des fins publicitaires ou commerciales tierces

## 3. Logs techniques

Les logs de l'hebergeur cloud contiennent uniquement :
- Acces HTTP au serveur de healthcheck (URL publique, sans identifiant
  utilisateur)
- Erreurs eventuelles du bot (stack traces techniques)

Ces logs sont conserves au maximum 7 jours par l'hebergeur et ne sont
accessibles qu'au proprietaire du bot.

## 4. Partage des donnees

yuAs69Bots ne partage AUCUNE donnee avec des tiers a des fins
commerciales. Les seuls services techniques externes utilises sont :

- **Discord** : interactions avec l'API du bot (obligatoire pour son
  fonctionnement)
- **MongoDB Atlas** : stockage chiffre au repos (donnees techniques)
- **Hebergeur cloud** : hebergement du bot 24/7

Aucun donnee n'est revendue, partagee a des fins publicitaires, ni
transferee hors UE/USA.

## 5. Tes droits (RGPD)

Si tu es citoyen de l'UE, tu as droit a :
- **Acces** : demander la liste de toutes tes donnees stockees
- **Suppression** : demander la suppression de tes donnees
- **Rectification** : demander la correction de donnees incorrectes
- **Portabilite** : recevoir tes donnees dans un format machine
- **Opposition** : t'opposer au traitement de tes donnees

Pour exercer ces droits : rejoins le [serveur Discord officiel](https://discord.gg/6RzwPAtFvq)
ou contacte **jibzz69** en DM Discord.

La commande `/botadmin resetserv` (reservee au proprietaire du bot)
permet de wiper toutes les donnees du bot pour un serveur en une fois.
Tu peux egalement quitter un serveur ou en retirer le bot pour que tes
donnees liees a ce serveur soient eligibles a suppression.

## 6. Duree de conservation

- **Donnees de configuration** : tant que le bot est present sur le
  serveur. Si le bot est retire, les donnees ne sont pas auto-supprimees
  immediatement mais peuvent l'etre sur demande.
- **Compteurs d'usage tier** : 60 jours (TTL MongoDB automatique)
- **Logs hebergeur** : 7 jours
- **Sessions de tickets** : selon politique d'archivage Discord du
  serveur concerne

## 7. Securite

- Toutes les donnees sont chiffrees au repos (MongoDB Atlas)
- Le code source du bot est prive et non distribue
- Acces a la base de donnees limite au proprietaire du bot uniquement
- Aucune authentification utilisateur n'est requise (Discord gere
  l'authentification via son OAuth)

## 8. Modifications

Cette politique peut etre modifiee a tout moment. Les changements
significatifs seront annonces sur le serveur officiel yuAs69Bots.

## 9. Contact

Pour toute question sur la confidentialite : rejoins le
[serveur Discord officiel](https://discord.gg/6RzwPAtFvq) ou contacte
**jibzz69** en DM Discord.
