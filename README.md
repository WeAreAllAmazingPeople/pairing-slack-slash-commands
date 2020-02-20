# pairing-slack-slash-commands
slash commands for a slack team that enable users to:
 - set themselves as available for code pairing (per channel)
 - for others to check who is available for pairing (per channel)
 - retrieve and keep statistics on pairing habits
 
 **/pairing** returns the list of people in the channel available for pairing 
          (per channel so you can use it as a differentiator/filter)
          
**/pairing** *yes*|*on*: mark yourself as available for pairing (for this channel)

**/pairing** *no*|*off*: mark yourself as unavailable for pairing (for this channel)

**/pairing-with** *@username*: mark yourself as pairing with a person

**/pairing-end**: mark your current pairing as finished

**/pairing-statistics**: should return statistics on a weekly basis, not yet implemented, 
                          functionality TBD.



## Heroku specific instructions
* Add Procfile
* Add requirements.txt file
* Add environment variable (Config Vars) "VERIFICATION_TOKEN"
* ~~Add environment variable (Config Vars) "DBNAME", "USERNAME" & "PASSWORD"~~
* Add add-on "heroku-postgresql"
** Config Var "DATABASE_URL" is added automatically by the add-on

## Slack instructions
* Browse to https://api.slack.com/apps and Create a New App
* Add Slash Commands
* Install to your workspace


