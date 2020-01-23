# ValkyriePerils
This is a event template for [Valkyrie](https://github.com/NPBruce/valkyrie/wiki).

Using this template you can easily add perils as used in Descent: Road to legend.

Manual:

1. Copy the perils.ini to your Valkyrie descent mission.
2. Add the perils.ini to the `[QuestData]` section of your quest.ini file.
3. Ensure your mission has an event which uses the `RoundEnd` trigger.
4. Add the `EventPerils` event to your RoundEnd-Trigger event.
5. Set the starting rounds for the perils by editing the PerilRound1-PerilRound6 variables.
6. Add a link event to your  RoundEnd-Trigger event the `EventEndPeril`.
