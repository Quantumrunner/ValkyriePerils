# ValkyriePerils
This is a event template for [Valkyrie](https://github.com/NPBruce/valkyrie/wiki).

Using this template you can easily add perils as used in Descent: Road to legend.

Manual:

1. Copy the perils.ini to your Valkyrie descent mission.
2. Add the perils.ini to the `[QuestData]` section of your quest.ini file.
3. Ensure your mission has an event which uses the `RoundEnd` trigger.
4. Add the `EventPerils` event to your RoundEnd-Trigger event.
5. Set the starting rounds for the perils by editing the `PerilRound1`-`PerilRound6` variables.
6. Set the button texts for the `EventPeril1button1`-`EventPeril1button1`, `EventPerils.button1` and the `EventEndPeril.button1` texts from the `Localization.English.txt` to the of `Localization.English.txt` your mission or add it from here:

`EventPerils.button1,Continue
EventEndPeril.button1,Continue
EventPeril1.button1,Continue
EventPeril2.button1,Continue
EventPeril3.button1,Continue
EventPeril4.button1,Continue
EventPeril5.button1,Continue
EventPerils6.button1,Continue`

7. Add a link event to your  RoundEnd-Trigger event the `EventEndPeril`.
