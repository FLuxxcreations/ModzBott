# ModzBott
Documentation for the ModzBott Discord bot.
Still require assistance? Visit the support server [here](https://discord.gg/ggdx5spFHF).

Here is a summary of the commands and features ModzBott has to offer:

### Server Logging:<br>
 **Current supported events:** <br>
`kick` - Logs member kicks from server<br>
`ban` - Logs member bans from server<br>
`timeout` - Logs member timeouts/mutes<br>
`role_change` - Logs role assignments/removals<br>
`nickname_change` - Logs nickname changes<br>
`message_delete` - Logs deleted messages<br>
`message_edit` - Logs edited messages<br>
`channel_purge` - Logs bulk message deletions<br>
`all` - All server events

**Logging commands:** <br>
<mark> **All server logging commands require the user to have the manage server commands. Users who do not have this permission will not be able to use it.** </mark>

`/logging enable` - Enables all logging for the server. This will create a <br>`#modzbott-logging` channel if a logging channel has not already been set or if the command has been used for the first time. 

`/logging disable` - Disables server logging entirely, but will retain logging settings for future use.

`/logging event [event_name] enable|disable` - Enable or disable a specific logging event. `event_name`: Supported events mentioned above. `enable` / `disable`: Toggles the event.

`/logging channel set|reset [channel]` - Assign a custom channel to log a specific event or reset it to the default channel.

`/logging cases view [case_id]` - View the details of a specific event case. This will return the ID, event (kick, ban etc.), target user, moderator, reason and the timestamp.

`/logging cases list` - Lists recent event cases.


### Moderation Commands:<br>
`/ban @member [reason]` – Ban a member from the server with an optional reason for logging. **Requires Ban Members permission.**

`/kick @member [reason]` – Kick a member from the server with an optional reason for logging. **Requires Kick Members permission.**

`/role [add/remove] [member] [@role]` – Add or remove roles from members quickly. **Requires Manage Roles permission.**

`/purge [messages]` – Delete up to 100 messages at once for fast cleanup. **Requires Manage Messages permission.**

`/slowmode [seconds]` – Set a slowmode on a channel to control message flow. **Requires Manage Channel permission.**

`/lockdown #channel` – Lock a channel to stop members from chatting or reacting. **Requires Manage Channels & Manage Roles permission.**

`/unlock #channel` – Unlock a previously locked channel to allow normal activity. **Requires Manage Channels & Manage Roles permission.**
<br><mark>Note - To unlock the channel after lockdown, the member needs the send messages permission in that channel. This can be done in the channel settings.</mark>

### Utility Commands:<br>
`/whois @member` – Get detailed information about any server member.

`/serverinfo` – Display general information about your server, including member count, roles, and more.

`/latency` – Check the current latency of ModzBott for fast troubleshooting.

`/invite` – Generate a link to invite ModzBott to your own server.

`/support` – Get a link to the official ModzBott Support Discord server.

### Fun & Engagement Commands:<br>
`/poll [question] [answer1] [answer2] [answer3] [answer4]` – Create a poll with up to 4 options to engage your community. Requires Create Poll permission.
