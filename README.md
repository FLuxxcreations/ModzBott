# ModzBott
Documentation for the ModzBott Discord bot.
Still require assistance? Visit the support server [here](https://discord.gg/ggdx5spFHF).

Here is a summary of the commands and features ModzBott has to offer:

### Welcome / Leave logging:<br>
**Current supported placeholders for custom messages:** <br>
`{member}` - Returns member name<br>
`{member_id}` - Returns member ID<br>
`{member_name}` - Same as {member}<br>
`{member_display}` - Shows the member's nickname if one exists (will show regular name if not)<br>
`{member_mention}` - Mentions the user<br>
`{guild_name}` - Server name<br>
`{guild_size}` - Member count after they join<br>

**Greeting commands:** <br>
<mark> **All greeting commands require the user and the bot to have the manage server commands. Users who do not have this permission will not be able to use it.** </mark>

`/greetings status` - Provides information on the server config for the module. 

`/greetings enable` - Enables all join / leave messages for the server. 

`/greetings disable` - Disables all join / leave messages for the server.

`/greetings event enable [event]` - Allows the user to enable join or leave only messages.

`/greetings event disable [event]` - Allows the user to disable join or leave only messages.

`/greetings channel [event] [#channel]` = Set a channel for either join logs or leave logs. 

`/greetings message preview [event]` - Preview how the join/leave message embed will appear in an active channel.

`/greetings message reset [event]` - Reset the custom join/leave message back to the default option.

`/greetings message set [event] [text]` - Set a custom message for when user joins or leaves.<br>**This does support the placeholders as mentioned above and Discord formatting. To start a new line, type \n then continue. For example, `Welcome to the server!\nWe hope you have a great time!`**

`/greetings dm enable` - Enables the bot to send welcome DMs to new members.

`/greetings dm disable` - Disables welcome DMs.

`/greetings dm set [text]` - Set a custom message for users to recieve when they join the server.<br>**This does support the placeholders as mentioned above and Discord formatting. To start a new line, type \n then continue. For example, `Welcome to the server!\nWe hope you have a great time!`**

`/greetings dm reset` - Reset the welcome DM to the defualt option.

`/greetings dm preview` - Preview how the welcome DM will be sent to members.

`/greetings autorole list` - View which roles will automatically be given to members when they join.

`/greetings autorole clear` - Stops adding roles to members when they join.

`/greetings autorole add @role1 @role2 @role3 etc.` - Add role(s) to be assigned to members when they join.

`/greetings autorole remove @role1 @role2 @role3 etc.` - Remove role(s) and stop them being assigned. 


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
<mark> **All server logging commands require the user and the bot to have the manage server commands. Users who do not have this permission will not be able to use it.** </mark>

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
