# Commands
## gameover
Triggers a Game Over.

## timerstop
Stops the timer.

**Aliases:** timestop, tstop, timerpause, timepause, tpause

## cap
Sets the state of the caps the player currently has.

**Arguments:** OPTION[invincible/vanish/metal/wing/none], wTOGGLE, *TIME

## ghostmode
Enables Ghostmode - invincibility, infinite fludd, noclip, no gravity.

**Aliases:** ghost

**Arguments:** wBOOL

## quit
Quits to the title screen.

**Aliases:** quitgame

## timerreset
Resets the timer and pauses until next transition

**Aliases:** timereset, treset, timerrestart, timerestart, trestart

## health
Sets a certain amount of health to the player. From 0 to 8.

**Aliases:** hp

**Arguments:** OPTION[NUMBER/refill/empty/death/infinity]

## clearhotkey
Clear a given hotkey.

**Aliases:** clhtk, chk, removehotkey, rmhtk, rhk

**Arguments:** KEY

## removecommand
Remove a command from a hotkey based on index (starting at 0) or the command

**Syntax:** removehotkey [key] [index/command]

Examples:
- /removecommand r 2
- /removecommand f warp 8-10

**Aliases:** clearcommand, rc, cc

**Arguments:** KEY, OPTION[NUMBER/STRING]
## setposition
Moves the player to the given position.

**Aliases:** setpos

**Arguments:** NUMBER, NUMBER

## lives
Sets the extra life counter.

**Arguments:** OPTION[NUMBER/infinity]

## coins
Sets the coin count.

**Aliases:** coin

**Arguments:** NUMBER

## exit
Exits the level.

**Aliases:** exitlevel

## reds
Sets the red coin count.

**Aliases:** red, redcoins, redcoin

**Arguments:** NUMBER

## camlock
Enables or disables camera edge locking.

**Aliases:** cl

**Arguments:** wTOGGLE

## file
Sets the contents of the current file to the specified profile.

**Aliases:** f

**Arguments:** OPTION[complete/essentials/empty]

## ldp
Trigger a Level Designer layer.

## char
Switches to the given character.

**Arguments:** OPTION[mario/luigi/toggle]

## resetcoins
Resets the coins position on the next loading zone.  Any of the additional options below will make spawned shines not despawn, thus not reactivating the shine spawn animation when reentering the room.

**Aliases:** restartcoins

**Arguments:** OPTION[preserveshinestate/preservestate/preserve/pres]

## timersplit
Triggers a timer split.  Can be used to split on certain actions.   

**Aliases:** timesplit, tsplit, split

**Arguments:** OPTION[onShine/onStarcoin/onJump/onDive/onRedCoin/onSilverStar/onRocket]

## animation
Sets the current character animation.

**Aliases:** anim

**Arguments:** NUMBER

## gravity
Sets gravity to the specified value.

**Aliases:** grav

**Arguments:** NUMBER

## fakebowser
Enables or disables the Fake Bowser fight.

**Aliases:** fb

**Arguments:** wTOGGLE

## setshine
Sets the state of the given shine ID.

**Aliases:** setstar, shine, star

**Arguments:** NUMBER, wTOGGLE

## zoomlock
Enables or disables zoom lock.

**Aliases:** zl

**Arguments:** wTOGGLE

## godmode
Enables Godmode - invincibility and infinite fludd.

**Aliases:** god

**Arguments:** wBOOL

## removewatch
Removes a variable watch.

**Aliases:** rw

**Arguments:** STRING

## showcollision
Makes collision visible as bright boxes.

**Aliases:** shc

**Arguments:** wTOGGLE

## doorwarp
Warps to a given door based on its internal ID.

**Aliases:** warpdoor, door

**Arguments:** STRING

## water
Sets the water tank value. From 0 to 10000.

**Arguments:** OPTION[refill/empty/infinity/NUMBER]

## fludd
Sets the availability state of FLUDD nozzles.

**Arguments:** OPTION[all/hover/rocket/turbo], wTOGGLE

## restartroom
Restarts the room from the spawn point.

**Aliases:** restart

## addwatch
Adds a variable watch.

**Aliases:** aw

**Arguments:** STRING

## hotkey
Add a hotkey for a given command.  Multiple commands can be added to the same hotkey and will be run in the order they were input unless otherwise specified in the command with the syntax ", [low/high/NUMBER] [WARNING: some commands will be overridden by others if they are inputted in the wrong order].  This can be done by either running hotkey multiple times on the same key or by separating the commands you with semicolons (no semicolon at the very end).  

Syntax: /hotkey [key] [command], *[priority]; [command], *[priority]; ... [command], *[priority]

Examples: 
- /hotkey r timerreset
- /hotkey w 8-10; timerreset; scf t
- /hotkey w 1-4; silvers 5; resetcoins, 0

**Aliases:** htk, hk

**Arguments:** KEY, STRING

## showwarps
Shows or hides warps (displayed as a black rectangle).

**Aliases:** sw

**Arguments:** wTOGGLE

## setvelocity
Sets the player's velocity.

**Aliases:** setspeed, setvel, sv

**Arguments:** OPTION[x/NUMBER], OPTION[y/NUMBER]

## bowserkey
Sets the state of a Bowser key.

**Aliases:** key, bk

**Arguments:** NUMBER, wTOGGLE

## showpecons
Shows or hides pecons.

**Aliases:** sp, pecons, pecon

**Arguments:** wTOGGLE

## silvers
Sets the silver star count.

**Aliases:** silver

**Arguments:** NUMBER

## air
Sets the remaining air. From 0 to 8.

**Arguments:** OPTION[refill/empty/infinity/NUMBER]

## timerstart
Starts the timer.

**Aliases:** timestart, tstart

## setstarcoin
Sets the state of the given starcoin ID.

**Aliases:** starcoin, sc

**Arguments:** NUMBER, wBOOL

## kill
Kills the player.

**Aliases:** die

## noclip
Enables or disables NoClip.

**Aliases:** nc

**Arguments:** wTOGGLE

## timer
Shows or hides the timer.

**Aliases:** time, timershow, timeshow, tshow

**Arguments:** wTOGGLE

## nozzleunlock
Sets the saved nozzles in a specific world.

**Aliases:** fluddunlock, nu, fludd

**Arguments:** OPTION[bob/sl/hmc/bm/lll/ttm/rr/bt3/ssl/wdw/ttc/all], OPTION[h/r/t/all], wTOGGLE

## warp
Warps the player to the specified room.  If no arguments are given, the warp command will default to the room and position set by the warpposition command

**Aliases:** w

**Arguments:** STRING:room_code, *NUMBER:x_pos, *NUMBER:y_pos, *STRING:transition_type, *BOOL:reset_music

## hidebg
Toggle hiding of the background layer.

**Aliases:** hbg

**Arguments:** wTOGGLE

## resetroom
Resets the room from the current position.

**Aliases:** reset, rr

## power
Sets the remaining fludd power. From 0 to 8.

**Aliases:** fluddpower

**Arguments:** OPTION[refill/empty/infinity/NUMBER]

## stage
Sets the player's world to the specified world.  Defaults to current room's world.

**Aliases:** setlevel, setstage, sl

**Arguments:** *STRING

## levelname
Returns the current room the player is in

**Aliases:** ln

## position
Returns the player's current position (x-coordinate, y-coordinate)

**Aliases:** pos

## showhotkey
Returns the current commands binded on the given hotkey

**Aliases:** shk, shtk

**Arguments:** String:key

## individuallevel
Sets up an individual level speedrun with the given parameters from the user.  Default is an 100% IL and all data about the stage will be reset(except for high score).  To add fludds, use a "-" for the last argument followed by h, r, t, or a(or any combination of them).  There are shortcuts for 100%(100), all star coins(asc), and all shines(as).  

Example: 
- /il bob as -a (start an all shines bob il with all fludds to start)

**Aliases:** il

**Arguments:** String:stage *Number:shines *Number:starcoins *String:fludds

## last
Runs the previous non-last command

**Aliases:** l

## setcurrentfludd
Changes the current fludd the player has equipped

**Aliases:** setfludd, scf, sf

**Arguments:** String:fludd

## cutscene
Enables or disables the cutscenes before and after True Bowser

**Aliases:** cs, cutscenes

**Arguments:** wTOGGLE

## resetdoors
Resets all unlockable castle doors so the shine/key animation will play on their next opening (assuming the player has the prerequisite shines/starcoins/key)

**Aliases:** resetdoor, rd

## lightningtransition
Makes the next transition a lightning transition(if possible).

**Aliases:** lt

## warpposition
Sets a default warp position for the warp command to your current position

**Aliases:** warpposition, warppos, wp

## delay
Runs a command after a user-given number of miliseconds

**Syntax:** /delay [miliseconds] [command]

**Arguments:** NUMBER, STRING
