# TeaMod

Tremulous server mod with bots

== ADMIN ==
It is controlled completely via admin commands:

!bot add [botname] [team]
!bot add ROBOCOP humans - adds ROBOCOP to human team
!bot add ALIENBOT aliens - adds ALIENBOT to alien team

!bot del [name-match]
!bot del ROBO - deletes every bot that contains 'ROBO' in their name
!bot del BOT - deletes every bot that contains 'BOT' in their name

!botcmd [name-match] [command]
This will change the bot behavior.
!botcmd ROBOCOP idle <-- idle. don't shoot enemy, nothing.
!botcmd ROBOCOP standground <-- stand ground but kill enemy.
!botcmd ROBOCOP regular <-- chase enemy and kill (default behavior).
!botcmd ROBOCOP teamkill <-- consider teammates as enemies.
!botcmd ROBOCOP followattack <-- follow me until you see enemy, kill it, then follow me again!
!botcmd ROBOCOP followidle <-- follow me no matter what. Do not attack.
!botcmd ROBOCOP followprotect <-- not yet implemented.
!botcmd ROBOCOP defensive <-- not yet implemented.
!botcmd ROBOCOP attack <-- not yet implemented.
!botcmd ROBOCOP skill [number] <-- Control Skill

Any other botcmd behavior will default to 'regular'.

== SETUP ==
OKAY, Pay attention. Your server MUST have reserved slots! In your config, you will find a line that looks like this (if not, add it!):

sv_privateclients 3

Change it's value (3) to the MAXIMUM amount of bots you want added!
The reserved password does not matter for bots.
