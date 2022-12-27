# 💲Activity Points

Every 30 seconds, you have the opportunity to win 1 activity point by sending a message into the Discord server

You can accumulate this points to level up in the activity levelling system TeriTeri includes. Every time you level up, you will get some tericoins and teristals as reward

# 🤖Commands

• `t!level channel <channel ID>` [Admin only]
> Sets the chosen channel as the place where TeriTeri sends the ñevel up notification messages

• `$alwaysReply`
> Detects every message that it's send on the server and gives the corresponding activity points and level ups, as well as including some other features on it, like some of the stigma sets boosts

• `t!set level boost <number>` [Admin only]
> Boosts the amount of activity points you get per message (max. 20/message)

• `t!check activity <@user>` [Admin only]
> Returns the amount of activity points the selected user has. It was created to make a user purge on the TeriTeriCult's new server

• `t!toggle ping <on/off>`
> Activates/deactives the level up mentions in the level up messages

# 📦Variables

• `point` [int]
> User var that saves the user's current activity points

• `level` [int]
> User var that saves the user's current level

• `level.channel` [int]
> Server var that saves the level up notifications channel ID

• `pts.cooldown` [int]
> User var that saves the timestamp of the last time the user got an activity point, to compare it to the current timestamp and see if they can get another point or not

• `lvl.boost` [int]
> Server var that saves the current level up boost. Set it to `0` to deactivate the level up system

• `lv.ping` [bool]
> User var that saves if you have the level up mentions active or not
