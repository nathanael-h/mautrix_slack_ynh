Un puente de marionetas entre Matrix y Slack empaquetado como un servicio YunoHost.
Mensajes, medios de comunicación y las notificaciones son puenteados entre una cuenta de Slack y una cuenta de Matrix.
Con la opción de inicio de sesión RelayBot, una persona de Matrix puede invitar a otra persona de Matrix a una sala de Slack puenteada, de modo que incluso personas sin cuenta de Slack pueden participar en conversaciones de grupo de Slack.
El puente ["Mautrix-Slack"](https://docs.mau.fi/bridges/go/slack/index.html) consiste en un servicio de la aplicación Synapse y se basa en Postgresql (Mysql también disponible).
Por lo tanto, debe instalarse previamente [Synapse para YunoHost](https://github.com/YunoHost-Apps/synapse_ynh).

** Atención: haz siempre copias de seguridad y restaura las aplicaciones Yunohost matrix_synapse y mautrix_slack juntas.