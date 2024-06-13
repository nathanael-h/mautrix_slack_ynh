<!--
Nota bene : ce README est automatiquement généré par <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
Il NE doit PAS être modifié à la main.
-->

# Matrix-Slack bridge pour YunoHost

[![Niveau d’intégration](https://dash.yunohost.org/integration/mautrix_slack.svg)](https://dash.yunohost.org/appci/app/mautrix_slack) ![Statut du fonctionnement](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.status.svg) ![Statut de maintenance](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.maintain.svg)

[![Installer Matrix-Slack bridge avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=mautrix_slack)

*[Lire le README dans d'autres langues.](./ALL_README.md)*

> *Ce package vous permet d’installer Matrix-Slack bridge rapidement et simplement sur un serveur YunoHost.*
> *Si vous n’avez pas YunoHost, consultez [ce guide](https://yunohost.org/install) pour savoir comment l’installer et en profiter.*

## Vue d’ensemble

Une passerelle entre Matrix et Slack empaquetée comme un service YunoHost.
Les messages, médias et notifications sont relayées entre un compte Slack et un compte Matrix.
Avec l'option de connexion Relaybot, un compte Matrix peut inviter d'autres comptes Matrix dans un salon Matrix relayé avec un groupe Slack, ainsi même des personnes sans compte Slack peuvent communiquer avec des utilisateur.ice.s de Slack.
La passerelle ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) consiste en un Service d'Application Matrix-Synapse et repose sur une base-de-données postgresql (mysql également possible).
C'est pourquoi [Synapse for YunoHost](https://github.com/YunoHost-Apps/synapse_ynh) doit être préalablemnet installé.

** Attention : sauvegardez et restaurez toujours les deux applications Yunohost matrix_synapse et mautrix_slack en même temps!**


**Version incluse :** 0.10.7~ynh1
## Documentations et ressources

- Site officiel de l’app : <https://maunium.net/go/mautrix-slack/>
- Documentation officielle de l’admin : <https://docs.mau.fi/bridges/go/slack/index.html>
- Dépôt de code officiel de l’app : <https://github.com/mautrix/slack>
- YunoHost Store : <https://apps.yunohost.org/app/mautrix_slack>
- Signaler un bug : <https://github.com/YunoHost-Apps/mautrix_slack_ynh/issues>

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche `testing`](https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing).

Pour essayer la branche `testing`, procédez comme suit :

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
ou
sudo yunohost app upgrade mautrix_slack -u https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
```

**Plus d’infos sur le packaging d’applications :** <https://yunohost.org/packaging_apps>
