# ValkyriePerils
This is an event template for creating peril events for [Descent: Journeys in the Dark (Second Edition)](https://descent2e.fandom.com) missions in the [valkyrie](https://github.com/NPBruce/valkyrie/wiki) mission creation tool.

Using this template you can easily add perils as used in Descent: Road to legend.

## What are perils?
Perils are encountered in Road to Legend / Valkyrie coop missions of descent. 

- Peril effects may occur at the end of a round after the heroes spent a certain amount of time in a quest or stage.
- Peril effects may cause monsters to spawn, deal damage, or generally inflict harm on the heroes.

Check out the  Descent [Community Rules Reference Guide (CRRG)](https://descent-community.org/index.php/crrg/) for more details regarding perils.

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
