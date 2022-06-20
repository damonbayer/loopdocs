# Medtronic Pump Users

## Prepare Medtronic Pump

!!! warning ""

    Before you begin the rest of the setup process, there are several steps on your Medtronic pump that you will need to complete prior to moving on with Loop setup. **DO NOT SKIP THESE STEPS OR YOUR LOOP WILL NOT WORK.**

1. Turn off Patterns under the basal menu settings. This will force Loop to use your "Standard" basal rate schedule.
2. Make sure your standard basal rate schedule is up-to-date and accurate. Loop will automatically import your pump's existing standard basal rate schedule when you add your pump in the subsequent parts of this page. **If you change basal rates later...make sure to make those changes in the Loop app and use Loop to save the changes back to the pump.  If you make changes directly in the pump, Loop will not automatically know about those changes and you will cause a mismatch.**
3. Set your pump's `Temp Basal Type` to `Insulin Rate (U/hr)`. Do NOT use percentage. Your Loop will not run unless your temp basal type is set to units/hour.
4. Make sure your maximum basal rate and maximum bolus (those are particular settings in the pump) are reasonably set for your particular needs. For new Loop users, a maximum basal rate equal to approximately 2-4 times your highest scheduled basal rate is a good starting point as you learn Loop and dial in your other settings. You can adjust as your comfort and use of Loop develop.
5. Set Remote Devices to `ON` and enter any random ID (010101 will work - avoid using all zeros). This setting is found in the pump's Utilities menu (for x23 continue to Connect Devices, Remotes) and turn `ON` the Remote Options.
6. Cancel any currently running extended or dual wave boluses.  Loop cannot loop with those running.
7. Make sure the other settings in your pump, such as bolus wizard settings, are up-to-date so that if you stop using Loop, those settings will be accurate for non-Loop traditional pump use.

## Connect Pump to Loop

**Section not yet edited for Loop 3.**


!!! warning ""
    New RileyLink compatible devices won't have a name listed next to their slider at first. The name will only be displayed after connecting the device to Loop for the first time. So, if all you see in the device list is a little toggle and no "RileyLink" name...go ahead and switch that toggle. The default device name will appear after that toggle is green.

    You can later [personalize](rileylink.md) the default device name once it is connected to Loop.

![img/pod-rl.png](../operation/loop-settings/img/pod-rl.png){width="400"}
{align="center"}

Continue with these steps to connect your Medtronic pump to Loop.  

1. Make sure your RileyLink is turned on and nearby, then you will see a RileyLink listed in this area of the settings.  Actually, you will see a list of any RileyLinks that are in the nearby area. Slide on the toggle for just one RileyLink.
2. Add your pump's region, color, and serial number. 
    * Note that some Canadian pumps use `CM` instead of `CA` for the region code.  Just select `CA` in the dropdown menu.
3. Click the `Continue` button to finish the addition of your pump.
<br/><br/>

![img/add_pump.png](../operation/loop-settings/img/add_pump.png){width="750"}
{align="center"}

!!! info "For x23 and x54 Medtronic pump users only"
    | <div style="width:144px"></div> ||
    |---|---|
    |![img/pump_broadcasts.png](../operation/loop-settings/img/pump_broadcasts.png){width="550"}|For x23 and x54 Medtronic pump users, there is a packet of information special to those pumps called MySentry messages. If you have never setup this part of the pump previously, you may see a screen, called "Pump Broadcasts", at this point in the setup process.</br></br>Follow the directions on the screen. They will require you to take some manual steps on your pump to "pair" it with your Loop app.</br></br>Basically, you will need to go to your pump's main menu, scroll down to Utilities, then Connect Devices, then Other Devices, turn that setting On, and then select Find Device. Once you do that, click on the `Continue` button in Loop app and the pairing will take place. This will allow those MySentry packets of information to flow to Loop app.</br></br>This step does not apply for x22 or x15 pump users, since those pumps do not have MySentry capabilities.|

Now that your pump is paired with Loop, you will be finishing these steps:

1. Change your pump time using the Loop app (and read all the info on that screen)
2. Import your pump's basal rate schedule, maximum basal rate, and maximum bolus (maximums are collectively called "delivery limits" in Loop)
3. Select your pump's battery type (lithium or alakine)
4. Leave the Preferred Data Source on Event History

**Event History must be selected for Nightscout to display temp basals, carbs, and boluses from Loop.**  Event History must also be selected in order for prime events to be detected and NOT contribute to IOB during site changes. Please just leave the Preferred Data Source on Event History.

![img/add_pump2.png](../operation/loop-settings/img/add_pump2.png){width="750"}
{align="center"}
