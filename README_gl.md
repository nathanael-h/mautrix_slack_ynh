<!--
NOTA: Este README foi creado automáticamente por <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
NON debe editarse manualmente.
-->

# Matrix-Slack bridge para YunoHost

[![Nivel de integración](https://dash.yunohost.org/integration/mautrix_slack.svg)](https://dash.yunohost.org/appci/app/mautrix_slack) ![Estado de funcionamento](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.status.svg) ![Estado de mantemento](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.maintain.svg)

[![Instalar Matrix-Slack bridge con YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=mautrix_slack)

*[Le este README en outros idiomas.](./ALL_README.md)*

> *Este paquete permíteche instalar Matrix-Slack bridge de xeito rápido e doado nun servidor YunoHost.*
> *Se non usas YunoHost, le a [documentación](https://yunohost.org/install) para saber como instalalo.*

## Vista xeral

A puppeting bridge between Matrix and Slack packaged as a YunoHost service.
Messages, media and notifications are bridged between a Slack user and a matrix user.
With the RelayBot login option, the matrix user can invite other matrix user in a bridged Slack room, such that even people without a Slack account can participate to Slack group conversations.
The ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) bridge consists in a synapse app service and relies on postgresql (mysql also available).
Therefore, [Synapse for YunoHost](https://github.com/YunoHost-Apps/synapse_ynh) should be installed beforehand.

** Attention: always backup and restore the Yunohost matrix_synapse et mautrix_slack apps together!**


**Versión proporcionada:** 0.10.7~ynh1
## Documentación e recursos

- Web oficial da app: <https://maunium.net/go/mautrix-slack/>
- Documentación oficial para admin: <https://docs.mau.fi/bridges/go/slack/index.html>
- Repositorio de orixe do código: <https://github.com/mautrix/slack>
- Tenda YunoHost: <https://apps.yunohost.org/app/mautrix_slack>
- Informar dun problema: <https://github.com/YunoHost-Apps/mautrix_slack_ynh/issues>

## Info de desenvolvemento

Envía a túa colaboración á [rama `testing`](https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing).

Para probar a rama `testing`, procede deste xeito:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
ou
sudo yunohost app upgrade mautrix_slack -u https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
```

**Máis info sobre o empaquetado da app:** <https://yunohost.org/packaging_apps>
