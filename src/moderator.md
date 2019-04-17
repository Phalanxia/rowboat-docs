# Moderator Command Quick-Reference

## Punishments

| Name | Description | Usage |
|------|-------------|-------|
| `;warn {user} [reason]` | Adds a warning infraction to a user | `;warn 232921983317180416 1st warning, spamming emoji` OR `;warn @rowboat#0001 2nd warning, going off-topic` |
| `;mute {user} [reason]` | Mutes a user. This will only work if `mute_role` is set in the config | `;mute 232921983317180416 spamming` OR  `;tempmute @rowboat#0001 60m spamming` |
| `;unmute {user}` | Unmutes a user | `;unmute 232921983317180416` |
| `;tempmute {user} {duration} [reason]` | Temporarily mutes a user. Will only work if `temp_mute_role` or `mute_role` is set in the config | `;tempmute 232921983317180416 30m spamming` OR `;tempmute @rowboat#0001 30m spamming` |
| `;kick {user} [reason]` | Kicks the user from the server | `;kick 232921983317180416 spamming` OR `;kick @rowboat#0001 spamming` |
| `;ban {user} [reason]` | Bans a user from the server | `;ban 232921983317180416 spamming` OR `;ban @rowboat#0001 spamming` |
| `;unban {user} [reason]` | Unbans a user | `;unban 232921983317180416` |
| `;forceban {User ID} [reason]` | Force bans a user who is not currently in the server | `;forceban 232921983317180416 spamming` |
| `;softban {user} [reason]` | Softbans (bans/unbans) a user and deletes the user's messages sent within the last 7 days | `;softban 232921983317180416 spamming` OR `;softban @rowboat#0001 spamming` |
| `;tempban {user} {duration} [reason]` | Temporarily bans a user | `;tempban 232921983317180416 5h spamming` OR `;tempban @rowboat#0001 5h spamming` |


## Admin Utilities

| Name | Description | Usage |
|------|-------------|-------|
| `;clean all [count]` | Cleans (deletes) [count] many messages in the current channel | `;clean all 20` |
| `;clean user {user} [count]` | Cleans [count] many messages a given user sent in the current channel | `;clean user 232921983317180416 50` |
| `;clean bots [count]` | Cleans [count] many messages sent by bots in the current channel | `;clean bots 30` |
| `;clean cancel` | Cancels any cleaning process running in current channel | `;clean cancel` |
| `;reactions clean {user} [count] [emoji]` | Removes the most recent count of reactions from a given user | `;reactions clean 232921983317180416` OR `;reactions clean @rowboat#0001 30` OR `;reactions clean 232921983317180416 20 :thinking:` |
| `;archive (here / all) [count]` | Archives [count] many messages in the current channel | `;archive all 50` OR `;archive here 50` |
| `;archive user {user} [count]` | Archives [count] many messages that a given user sent in the current guild | `;archive user 232921983317180416 100` OR `;archive user @rowboat#0001 100` |
| `;archive channel {channel} [count]` | Archives [count] many messages in the given channel | `;archive channel 289482554250100736 20` |
| `;search {query}` | Searches for usernames that match given query | `;search b1nzy` |
| `;voice log {user}` | Displays a list of a given user's recent voice channel activity | `;voice log 232921983317180416` OR `;voice log @rowboat#0001` |
| `;test_filter {string}` | Returns a list of words detected by the text filter | `;test_filter You're a noob!` |


## Infractions

| Name | Description | Usage |
|------|-------------|-------|
| `;infractions search {query}` | Searches infractions database for given query | `;infractions search 232921983317180416` OR `;infractions search rowboat#0001` OR `;infractions search spamming`
| `;infractions info {inf#}` | Presents information on the given infraction | `;infractions info 1274`
| `;infractions duration {inf#} {duration}` | Updates the duration of the given infraction. Duration starts from time of initial action | `;infractions duration 1274 5h` |
| `;infractions reason {inf#} {reason}` | Updates the reason of a given infraction | `;infractions reason 1274 rude behaviour towards staff` |
