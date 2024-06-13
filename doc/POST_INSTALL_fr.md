## Liste de passerelles publiques
* Demandez sur un des salons suivants: #mautrix_yunohost:matrix.fdn.fr or #slack:maunium.net

## Usages de la passerelle
** Notez que plusieurs comptes Slack et Matrix peuvent être relayés, chaque compte Slack connecté a son propre salle d'Administration. Si plusieurs utilisateur.ice.s du Robot sont dans un même groupe Slack, seul une salle Matrix sera créé par la passerelle. **

### Relayer TOUTES les conversations entre UN compte Slack et UN compte Matrix
* Prérequis : votre compte Matrix ou le serveur sur lequel il est hébergé doit être autorisé dans la configuration de la passerelle (voir ci-dessous)
* Invitez le Robot (par défaut @slackbot:synapse.votredomaine) à une nouvelle conversation.
* Cette nouveau salle d'administration du Robot Mautrix-Slack est appelé "Administration Room".
* Tapez `login`
* Scannez le QR-code avec la caméra Slack de votre Machine Virtuelle ou ordiphone (option Slack Web dans l'appli)
* Envoyez `help` au Robot dans le "Administration Room" pour une liste des commandes d'administration de la passerelle.
  Voir aussi [upstream wiki Authentication page](https://docs.mau.fi/bridges/go/slack/authentication.html)

### Passerelle vers une conversation existante
Par défaut, la passerelle crée une salle pour chaque groupe Slack que l'utilisateur Slack utilise activement.
Vous pouvez également créer un portail pour une salle Matrix existante. **Notez qu'il peut s'agir d'une salle créée par une autre passerelle, par exemple une salle de portail Signal.
1. Invitez le bot de la passerelle dans la salle (avec un utilisateur autorisé).
2. Tapez `!wa create`
3. Votre utilisateur connecté crée un nouveau groupe correspondant.
4. Obtenez le lien d'invitation `!wa invite-link` et partagez-le avec vos amis. Ou invitez les marionnettes Slack dans la pièce.
5. Facultatif : Activez le relaybot, voir la section suivante.

### Relaybot: Relayer les conversations de TOUS les comptes Matrix et TOUS les comptes Slack présents dans UN groupe/salle
1. Activer l'option `Should Relay Mode be allowed?` dans le panneau de configuration (section `Main Settings -> Puppetting Bridge Settings`) ou dans le fichier YAML de configuration du robot `relay: enabled: true`. Assurez-vous également que les utilisateurs que vous voulez inviter ont au moins le niveau `relay` dans la section `permissions` (ceci peut être configuré dans la section `Main Settings -> Permissions for using the bridge` du panneau de configuration).
2. Connectez-vous à votre compte Slack dans la salle d'administration.
2. En fonction de ce qui a été sélectionné lors de l'installation, cela peut être fait uniquement par les administrateurs, mais peut également être modifié dans la section `Main Settings -> Puppetting Bridge Settings` du panneau de configuration ou dans le fichier YAML de configuration du robot `relay: admin_only`
3. Ecrivez `!wa set-relay` dans chacune des pièces que vous voulez relayer pour (ré)activer la fonction de relaybot.

* Vous pouvez maintenant relayer un groupe Slack en y invitant le numéro de téléphone du compte Slack connecté au Relaybot. Côté Slack, tous les messages venant de Matrix seront vus comme envoyés depuis le compte Slack connecté, avec un préfix indiquant le compte Matrix correspondant. Côté Matrix, la passerelle va créer des comptes Matrix pour chaque compte Slack présent dans le groupe relayé. Les messages sont indiqués comme provenant soit du numéro de téléphone, soit du pseudo Slack.
  Voir aussi [la page wiki principale sur le Relaybot](https://docs.mau.fi/bridges/go/slack/relaybot.html)