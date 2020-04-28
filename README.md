# ValkyriePerils
This is a event template for [Valkyrie](https://github.com/NPBruce/valkyrie/wiki).

Using this template you can easily add perils as used in Descent: Road to legend.

## How to use the template:

1. Copy the perils.ini to your Valkyrie descent mission.

![PerilIniScreenshot](/Images/perilIni.png)

2. Add the perils.ini to the `[QuestData]` section of your quest.ini file.

![QuestIniScreenshot](/Images/QuestIni.png)

3. Ensure your mission has an event which uses the `RoundEnd` trigger. Add an `EndRoundEvent` as a follow up event. Assign the variable `PerilDone` to 0.

![EndRoundTriggerScreenshot](/Images/EndRoundTrigger.png)

4. Add the `EventPerils` event to your RoundEnd-Trigger event.

![EndRoundEventsScreenshot](/Images/EndRoundEvents.png)

5. Set the starting rounds for the perils by editing the `PerilRound1`-`PerilRound6` variables.

![PerilVariablesScreenshot](/Images/PerilVariables.png)

6. Add a link event to your  RoundEnd-Trigger event the `EventEndPeril`.

![EndPerilScreenshot](/Images/EndPeril.png)

If everything worked correctly a peril text should appear at the end of the next round:

![EndPerilScreenshot](/Images/Peril1.png)
