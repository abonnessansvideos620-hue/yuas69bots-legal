# Politique de confidentialite de yuAs69Bots

*Derniere mise a jour : 14 mai 2026*

## 1. Donnees collectees

yuAs69Bots collecte et stocke uniquement les donnees necessaires a son
fonctionnement, dans une base MongoDB Atlas chiffree au repos.

### Donnees stockees par fonctionnalite

| Fonctionnalite | Donnees |
|---|---|
| **Levels (XP)** | guild_id, user_id, xp, niveau, derniere activite |
| **Auto-reponses** | guild_id, trigger, reponse, createur |
| **Commandes custom** | guild_id, nom, reponse, createur |
| **Giveaways** | guild_id, message_id, prix, gagnants, liste des participants |
| **Reaction roles** | guild_id, message_id, mapping emoji -> role |
| **Suggestions** | guild_id, message_id, auteur, texte, liste des votants up/down, statut |
| **Rappels** | user_id, texte, date programmee |
| **Newsletter (pub)** | guild_id, user_id (subscribers) |
| **Anti-raid / Anti-spam** | guild_id, configuration (pas de log des actions) |
| **Verification** | guild_id, channel_id, role_ids |
| **Tier premium** | guild_id, tier, date d'expiration |
| **Welcome DM** | guild_id, message de bienvenue |

## 2. Donnees NON collectees

yuAs69Bots ne collecte JAMAIS :
- Le contenu des messages prives (DMs) entre utilisateurs
- Le contenu des messages des salons hors triggers explicites
- Les mots de passe, emails, ou IP
- Aucune donnee a des fins publicitaires ou de revente

## 3. Logs

Les logs Render (techniques) contiennent les acces HTTP au serveur
keepalive et les erreurs eventuelles. Ces logs sont conserves 7 jours
maximum par Render et ne sont pas accessibles par des tiers.

## 4. Partage des donnees

yuAs69Bots ne partage AUCUNE donnee avec des tiers. Les seuls services
externes utilises sont :
- **Discord** : pour les interactions avec l'API (obligatoire)
- **MongoDB Atlas** : pour le stockage (chiffre au repos)
- **Render** : pour l'hebergement
- **UptimeRobot** : ping HTTP toutes les 5 min (uniquement l'URL de
  healthcheck, aucune donnee utilisateur)
- **Stripe** *(si applicable)* : pour le paiement premium (Stripe gere
  les donnees de carte, yuAs69Bots ne les voit jamais)

## 5. Tes droits (RGPD)

Si tu es citoyen de l'UE, tu as droit a :
- **Acces** : demander la liste de toutes tes donnees stockees
- **Suppression** : demander la suppression de tes donnees
- **Rectification** : demander la correction de donnees incorrectes
- **Portabilite** : recevoir tes donnees dans un format machine

Pour exercer ces droits : rejoins le [serveur Discord officiel](https://discord.gg/6RzwPAtFvq)
ou contacte le proprietaire (jibzz69) en DM. Une commande `/botadmin resetserv`
permet aussi a l'admin du serveur de wiper toutes les donnees du bot pour son
serveur en une fois.

## 6. Duree de conservation

- **Donnees de configuration** : tant que le bot est present sur le
  serveur. Si le bot est retire, les donnees ne sont pas auto-supprimees
  immediatement mais peuvent l'etre sur demande.
- **Compteurs d'usage tier** : 60 jours (TTL MongoDB automatique)
- **Logs Render** : 7 jours

## 7. Modifications

Cette politique peut etre modifiee a tout moment. Les changements
significatifs seront annonces sur le serveur officiel yuAs69Bots.

## 8. Contact

Pour toute question sur la confidentialite : rejoins le
[serveur Discord officiel](https://discord.gg/6RzwPAtFvq) ou contacte
le proprietaire (jibzz69) en DM.
