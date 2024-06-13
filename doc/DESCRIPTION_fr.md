Une passerelle entre Matrix et Slack empaquetée comme un service YunoHost.
Les messages, médias et notifications sont relayées entre un compte Slack et un compte Matrix.
Avec l'option de connexion Relaybot, un compte Matrix peut inviter d'autres comptes Matrix dans un salon Matrix relayé avec un groupe Slack, ainsi même des personnes sans compte Slack peuvent communiquer avec des utilisateur.ice.s de Slack.
La passerelle ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) consiste en un Service d'Application Matrix-Synapse et repose sur une base-de-données postgresql (mysql également possible).
C'est pourquoi [Synapse for YunoHost](https://github.com/YunoHost-Apps/synapse_ynh) doit être préalablemnet installé.

** Attention : sauvegardez et restaurez toujours les deux applications Yunohost matrix_synapse et mautrix_slack en même temps!**
