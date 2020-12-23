# ValkyriePerils
This is an event template for creating peril events for [Descent: Journeys in the Dark (Second Edition)](https://descent2e.fandom.com) missions in the [valkyrie](https://github.com/NPBruce/valkyrie/wiki) mission creation tool.

Using this template you can easily add perils to your valkyrie missions as used in [Descent: Road to legend](https://www.fantasyflightgames.com/en/news/2016/3/15/road-to-legend/).

## What are perils?
Perils are encountered in Descent: Road to Legend / Valkyrie coop missions of descent. 

- Peril effects may occur at the end of a round after the heroes spent a certain amount of time in a quest or stage.
- Peril effects may cause monsters to spawn, deal damage, or generally inflict harm on the heroes.

Check out the  Descent [Community Rules Reference Guide (CRRG)](https://descent-community.org/index.php/crrg/) for more details regarding perils.

Valkyrie contains three forms of perils:

- minor
- major
- deadly

**Minor perils** only have a minor negative effect for the heroes (e.g. poisoning a hero). **Major perils** can have heavy negative effects for the heroes and kill heroes if the heroes are not well prepared (e.g. 4 damage to all heroes). **Deadly perils** end a mission after a specific number of rounds or make a huge amount of damage. The problem with these kind of perils is that you can not react to them. The app doesn't tell you as app developer when the deadly peril which ends the game happens. **Therefore do not use this perils at all!** Instead create custom events when you want to use deadly peril effects.

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
