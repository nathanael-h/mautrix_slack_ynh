<!--
Este archivo README esta generado automaticamente<https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
No se debe editar a mano.
-->

# Matrix-Slack bridge para Yunohost

[![Nivel de integración](https://dash.yunohost.org/integration/mautrix_slack.svg)](https://dash.yunohost.org/appci/app/mautrix_slack) ![Estado funcional](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.status.svg) ![Estado En Mantención](https://ci-apps.yunohost.org/ci/badges/mautrix_slack.maintain.svg)

[![Instalar Matrix-Slack bridge con Yunhost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=mautrix_slack)

*[Leer este README en otros idiomas.](./ALL_README.md)*

> *Este paquete le permite instalarMatrix-Slack bridge rapidamente y simplement en un servidor YunoHost.*
> *Si no tiene YunoHost, visita [the guide](https://yunohost.org/install) para aprender como instalarla.*

## Descripción general

Un puente de marionetas entre Matrix y Slack empaquetado como un servicio YunoHost.
Mensajes, medios de comunicación y las notificaciones son puenteados entre una cuenta de Slack y una cuenta de Matrix.
Con la opción de inicio de sesión RelayBot, una persona de Matrix puede invitar a otra persona de Matrix a una sala de Slack puenteada, de modo que incluso personas sin cuenta de Slack pueden participar en conversaciones de grupo de Slack.
El puente ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) consiste en un servicio de la aplicación Synapse y se basa en Postgresql (Mysql también disponible).
Por lo tanto, debe instalarse previamente [Synapse para YunoHost](https://github.com/YunoHost-Apps/synapse_ynh).

** Atención: haz siempre copias de seguridad y restaura las aplicaciones Yunohost matrix_synapse y mautrix_slack juntas.

**Versión actual:** 0.10.7~ynh1
## Documentaciones y recursos

- Sitio web oficial: <https://maunium.net/go/mautrix-slack/>
- Documentación administrador oficial: <https://docs.mau.fi/bridges/go/slack/index.html>
- Repositorio del código fuente oficial de la aplicación : <https://github.com/mautrix/slack>
- Catálogo YunoHost: <https://apps.yunohost.org/app/mautrix_slack>
- Reportar un error: <https://github.com/YunoHost-Apps/mautrix_slack_ynh/issues>

## Información para desarrolladores

Por favor enviar sus correcciones a la [`branch testing`](https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing

Para probar la rama `testing`, sigue asÍ:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
o
sudo yunohost app upgrade mautrix_slack -u https://github.com/YunoHost-Apps/mautrix_slack_ynh/tree/testing --debug
```

**Mas informaciones sobre el empaquetado de aplicaciones:** <https://yunohost.org/packaging_apps>
