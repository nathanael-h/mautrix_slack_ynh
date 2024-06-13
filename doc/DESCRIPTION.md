A puppeting bridge between Matrix and Slack packaged as a YunoHost service.
Messages, media and notifications are bridged between a Slack user and a matrix user.
With the RelayBot login option, the matrix user can invite other matrix user in a bridged Slack room, such that even people without a Slack account can participate to Slack group conversations.
The ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) bridge consists in a synapse app service and relies on postgresql (mysql also available).
Therefore, [Synapse for YunoHost](https://github.com/YunoHost-Apps/synapse_ynh) should be installed beforehand.

** Attention: always backup and restore the Yunohost matrix_synapse et mautrix_slack apps together!**
