## List of known public services
* Ask on one of the following rooms: #mautrix_yunohost:matrix.fdn.fr or #slack:maunium.net

## Bridging usage
** Note that several Slack and Matrix users can be bridged, each Slack account has its own bot administration room. If they are in a same Slack group, only one matrix room will be created. **

### Bridge a Slack user and a Matrix user
* First your matrix user or server has to be authorized in the bridge configuration (see below)
* Then, invite the bot (default @slackbot:yoursynapse.domain)
* The room with the Mautrix-Slack bot is called "administration room".
* Type `login`
* Capture the QR code with the camera in the Slack of your VM or smartphone (Slack Web)
* Send `help` to the bot in the created room to know how to control the bot.
  See also [upstream wiki Authentication page](https://docs.mau.fi/bridges/go/slack/authentication.html)

### Bridge an existing room
By default, the bridge creates a room for each Slack group that the Slack user actively uses.
Your can also create a portal for an existing Matrix room. **Note that this can be a room created by another bridge, e.g. a Signal room**
1. Invite the bridge bot to the room (with an authorized user)
2. Type `!wa create`
3. Your logged-in user creates a new corresponding group.
4. Get the invite link `!wa invite-link` and share it with friends. Or invite Slack puppets to room.
5. Optional: Activate relaybot, see next section.

### Relaybot: Bridge a group for several Matrix and several Slack users to chat together
To be able to bridge not only your logged in Matrix account but also Matrix friends you invite to a room, you need to:
1. Enable relaybot setting in the config panel section `Main Settings -> Puppetting Bridge Settings` or in the bridge configuration YAML file `relay: enabled: true`. Also make sure that the users you want to invite have at least the `relay` level in the `permissions` section (this can be configured in the config panel section `Main Settings -> Permissions for using the bridge`).
2. Login to your Slack account in the (main) administration room
3. Depending on what has been selected during installation this could be done only by admins, but can also be changed in the config panel section `Main Settings -> Puppetting Bridge Settings` or in the bridge configuration YAML file `relay: admin_only`.
4. Write `!wa set-relay` in each of the rooms you want to relay to (re-)activate the relaybot function.

* In Slack: all messages will be seen as received from the account who is logged in with a prefix for the source Matrix user.
* On the Matrix side: the bridge will create matrix puppets corresponding to the Slack users when they send a message.
  See also [upstream wiki Relaybot page](https://docs.mau.fi/bridges/general/relay-mode.html)