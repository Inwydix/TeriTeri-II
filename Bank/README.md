# 馃彟 Server Bank

The server bank is a place where everyone in the server can save tericoins to obtain rewards. These rewards are available to everyone in the server once a certain number of tericoins are stored in the bank

Note: no one can withdraw money from the bank

# 馃 Commands

路 `t!create bank` [Admin only]
> Creates a voice channel to be the server bank

路 `t!set bank channel <channel ID>` [Admin only]
> Sets the selected channel as the place where people can see how many tericoins are in the bank. Link the voice channel you created using this 

路 `t!` 
> Every time someone makes a command, checks if a new bank milestone was reached and sends a message notifying it

路 `t!add bank <amount>` 
> Adds the chosen amount of tericoins to the server bank. It has a cooldown of 1 second per every 10 tericoins added, with a minimun cooldown of 10 minutes.
> It also updates the value shown in the server bank channel

# 馃摝 Variables

路 `bank` [int]
> Server var that saves the amount of tericoins the bank currently has

路 `bankID` [int]
> Server var that saves the ID of the bank channel

路 `bank.prog` [int]
> Server var that saves the current bank milestone. It's used to check if you can do x things that unlocks with each milestone

路 `bank.worker` [int]
> Server var that saves the amount of extra workers of each type unlocked with the bank milestones

路 `bank.cd` [imrpo array]
> Server var that saves the timestamp of the last time someone added tericoins to the bank/the amount of seconds the cooldown has depending on how many tericoins that person added to the bank
> 
> Looks like [timestamp/seconds] 
