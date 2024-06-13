<!--
Ohart ongi: README hau automatikoki sortu da <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>ri esker
EZ editatu eskuz.
-->

# Matrix-Slack bridge YunoHost-erako

[![Integrazio maila](https://dash.yunohost.org/integration/mautrix_slack.svg)](https://dash.yunohost.org/appci/app/mautrix_slack) ![Funtzionamendu egoera](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.status.svg) ![Mantentze egoera](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.maintain.svg)

[![Instalatu Matrix-Slack bridge YunoHost-ekin](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=mautrix_slack)

*[Irakurri README hau beste hizkuntzatan.](./ALL_README.md)*

> *Pakete honek Matrix-Slack bridge YunoHost zerbitzari batean azkar eta zailtasunik gabe instalatzea ahalbidetzen dizu.*
> *YunoHost ez baduzu, kontsultatu [gida](https://yunohost.org/install) nola instalatu ikasteko.*

## Aurreikuspena

A puppeting bridge between Matrix and Slack packaged as a YunoHost service.
Messages, media and notifications are bridged between a Slack user and a matrix user.
With the RelayBot login option, the matrix user can invite other matrix user in a bridged Slack room, such that even people without a Slack account can participate to Slack group conversations.
The ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) bridge consists in a synapse app service and relies on postgresql (mysql also available).
Therefore, [Synapse for YunoHost](https://github.com/YunoHost-Apps/synapse_ynh) should be installed beforehand.

** Attention: always backup and restore the Yunohost matrix_synapse et mautrix_slack apps together!**


**Paketatutako bertsioa:** 0.10.7~ynh1
## Dokumentazioa eta baliabideak

- Aplikazioaren webgune ofiziala: <https://maunium.net/go/mautrix-slack/>
- Administratzaileen dokumentazio ofiziala: <https://docs.mau.fi/bridges/go/slack/index.html>
- Jatorrizko aplikazioaren kode-gordailua: <https://github.com/mautrix/slack>
- YunoHost Denda: <https://apps.yunohost.org/app/mautrix_slack>
- Eman errore baten berri: <https://github.com/YunoHost-Apps/mautrix_slack_ynh/issues>

## Garatzaileentzako informazioa

Bidali `pull request`a [`testing` abarrera](https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing).

`testing` abarra probatzeko, ondorengoa egin:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
edo
sudo yunohost app upgrade mautrix_slack -u https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
```

**Informazio gehiago aplikazioaren paketatzeari buruz:** <https://yunohost.org/packaging_apps>
