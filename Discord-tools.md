[Home](Home.md)

***

Bippity currently provides a small number of tools to aid in running ttrpg sessions.

# Scheduling
The `/schedule` command can be used to create discord's custom formatted timestamps counting down to the date of your next event. To use it, type `/schedule` and then either the unix timestamp for the start of the next event, or the number of weeks after the previous event at which you wish to schedule the next one. This will output the countdown in the format `Next session will be on [day, date, time], in [time until event]`.

When specifying a unix timestamp, it will simply copy this into its formula. When specifying number of weeks however, it will first search the channel where the command was run for the latest message sent in its output format, then calculate a timestamp after that by the exact number of weeks provided. The weeks features will therefore only work if a similar message to its output already exists in the channel, either by manually writing it, or by providing a raw timestamp.

# Dice Rolling
Bippity is able to roll d6s when asked. the `/r` command will generate a random number from 1 to 6, then, if a modifier is also passed to the command, add this to the generated number, and output the result.

The `/a` and `/d` commands function the same, with the exception that 2 numbers are randomly generated, but only the lower or higher number is used for the calculation and output, respectively. This is meant to mirror the concept of "advantage" and "disadvantage". 
