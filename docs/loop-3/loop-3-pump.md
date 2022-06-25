# Pump Configuration

## Pump Choices

The pump configuration can be selected from the Heads-Up-Display ([HUD](loop-3-displays.md#heads-up-display)) or from the [Loop Settings](loop-3-settings.md) screen.

The HUD will look like the graphic below if no CGM or Pump is configured for Loop:

![Loop HUD when both CGM and Pump have not been added](img/loop-3-hud-add-cgm-add-pump.svg){width="350"}
{align="center"}

!!! question "Switching Pumps?"
    If you already have a pump connected to Loop and want to switch to a different pump, go to [Modify Pump](#modify-pump).

Loopers can choose from 3 pumps and a simulator:

* Minimed 500/700 Series
* Omnipod
* Omnipod DASH
* Insulin Pump Simulator

!!! info "Omnipod vs Omnipod DASH"
    Insulet uses the term Omnipod to refer to the older (Eros) pods.

    Insulet uses the term Omnipod DASH to refer to newer BLE DASH pods.

    The Loop app follows this convention. LoopDocs uses:

    * **Omnipod**: specific to the older (Eros) pods that require a RileyLink compatible device
    * **Omnipod DASH**: specific to the new BLE pods
    * **Omnipod Common**: refers to information that is common to both types of pods


## Add Pump

The graphic below shows the display when a user taps on Add Pump in the Settings screen. Tap on the desired Pump to advance to the next screen.

![graphic showing the pumps available with Loop 3](img/loop-3-setting-add-pump.svg){width="500"}
{align="center"}


If you are adding a Medtronic pump, skip ahead to [Insulin Type](#insulin-type).

## Omnipod Common

### Pod Nofication Defaults

The graphics below show the common screens for adding Omnipod or Omnipod DASH. These are the default notifications used for all future pods. These default settings can be modified later.

![initial screens for pod set up to define default notifications](img/loop-3-pod-notification.svg){width="600"}
{align="center"}

After these screens are completed, the insulin type is selected.

## Insulin Type

The insulin type screen is presented for all pumps.

* Insulin Type
    * User can select from Rapid (Novolog, Humalog, Apidra) or Ultra-Rapid (Fiasp, Lyumjev)
    * For Rapid insulin, the [Child or Adult](loop-3-therapy.md#insulin-model) model selection made in Therapy Settings is used
    * For the Ultra-Rapid insulin, only one model is available
    * Inhaled insulin (Afrezza) is not suitable for pump use so is not offered at this screen; it is only available for use with [Non-Pump Insulin](loop-3-displays.md#event-history-reservoir-and-non-pump-insulin)

![initial selection for insulin used in pump](img/loop-3-add-pump-insulin.svg){width="250"}
{align="center"}

After this screen is presented, [Omnipod DASH](#omnipod-common_1) users should skip ahead - they will not use a RileyLink compatible device.

## Omnipod or Medtronic

### Select RileyLink

For Omnipod and Medtronic pumps, a RileyLink compatible device is required for Loop to control your pump. You will learn to make it a habit to keep that device and your phone within range of your pump to keep Loop a nice green color.

!!! warning ""
    New RileyLink compatible devices won't have a name listed next to their slider at first. The name will only be displayed after connecting the device to Loop for the first time. So, if all you see in the device list is a little toggle and no "RileyLink" name...go ahead and switch that toggle. The default device name will appear after that toggle is green.

    You can later [personalize](../operation/loop-settings/rileylink.md) the default device name once it is connected to Loop.

![img/pod-rl.png](../operation/loop-settings/img/pod-rl.png){width="400"}
{align="center"}

A list of all RileyLink compatible devices in the nearby area will display in the RileyLink Setup screen. Select your RileyLink by sliding the toggle to display green and then press the blue `Continue` button at the bottom of the screen. 

If your device does not appear:

* Make sure it is charged and turned on
* Make sure it is not still connected to a different phone or app

Click this link to continue with a [Medtronic](#medtronic) pump.

## Omnipod Common

After the detour for selecting a RileyLink for Omnipod, all other actions for Omnipod and Omnipod DASH are the same. Once a pod is paired, the Pump display will be the same, except the Omnipod screen has a section for the RileyLink Devices.

### Pod Pairing

A [video is found here for pairing an Omnipod DASH pod](https://drive.google.com/file/d/1mN5s8-oorvoa-gbjAaYbnUnl_-vvuhNC/view?usp=sharing). Once the pod starts priming, you may want to skip ahead in the video (priming takes a minute to complete). The Omnipod Common pairing protocol is the same. The difference is that Omnipod requires a RileyLink compatible device and Omnipod DASH does not. There are also slight differences in some of the text, e.g., Omnipod DASH uses a blue needle cap and Omnipod has a clear needle cap.


## Medtronic

If you've been following this page to add your Medtronic pump, you have completed the first three steps.  If not, you can prepare your pump now, then do those first three steps using Loop (follow the links). The final Connect the Pump step requires all other steps be completed first.

1. Select [Minimed 500/700 Series](#add-pump) as your pump
1. Select [Insulin Type](#insulin-type)
1. Select [RileyLink](#select-rileylink)
1. [Prepare Medtronic Pump](#prepare-medtronic-pump)
1. [Connect Pump to Loop](#connect-pump-to-loop)

### Prepare Medtronic Pump

!!! warning ""

    **These steps are required for your Medtronic pump to work with Loop. Check with your users guide (can be found online if you don't have one) for more detailed instructions on your model of pump if you're not sure how to accomplish these steps.**

1. Turn off Patterns under the basal menu settings.
2. If you have basal rates, insulin to sensitivity factor and carb ratios in your pump - these will be overwritten (using the Therapy Setting values) when you connect your pump to Loop. If those rates are important to you, record them prior to continuing.
1. Set the Max Basal and Max Bolus values in the Medtronic pump to be greater than or equal to the values you enter in the Loop [Therapy Settings](loop-3-therapy.md#delivery-limits). Otherwise, Loop will not connect to your pump with the error message: `Pump Error. Max setting exceeded`.
3. Set your pump's `Temp Basal Type` to `Insulin Rate (U/hr)`. Do NOT use percentage. Loop will not run unless your temp basal type is set to units/hour.
5. Set Remote Devices to `ON` and enter any random ID (010101 will work - avoid using all zeros). This setting is found in the pump's Utilities menu (for x23 continue to Connect Devices, Remotes) and turn `ON` the Remote Options.
6. Cancel any currently running extended or dual wave boluses.  Loop cannot loop with those running.
7. Make sure the other settings in your pump, such as bolus wizard settings, are up-to-date so that if you stop using Loop, those settings will be accurate for non-Loop traditional pump use.

### Connect Pump to Loop

After all other steps are completed, you can connect your Medtronic pump to Loop.  

1. Make sure your RileyLink is turned on and nearby.
2. Add your pump's region, color, and serial number. 
    * Note that some Canadian pumps use `CM` instead of `CA` for the region code.  Select `CA/CM` in the dropdown menu.
3. Click the `Continue` button to connect the pump to Loop.
    - If the [Delivery Limits](loop-3-therapy.md#delivery-limits) (max basal and max bolus) in the pump are lower than values you entered in Loop you will see an error message: `Pump Error. Max setting exceeded`.
    - In this case, edit the values in the pump and click `Continue` to retry (this is faster than quitting, modifying Loop settings and then restarting this process).
1. You will then be presented with a Pump Clock message, click the `Continue` button
1. Finally you get a `Pump is ready for use screen`, click the `Continue` button
1. If you have an x23 or x54 pump, there is one more step - highlighted below
<br/><br/>

![img/add_pump.png](../operation/loop-settings/img/add_pump.png){width="750"}
{align="center"}

!!! info "For x23 and x54 Medtronic pump users only"
    | <div style="width:144px"></div> ||
    |---|---|
    |![img/pump_broadcasts.png](../operation/loop-settings/img/pump_broadcasts.png){width="550"}|For x23 and x54 Medtronic pump users, there is a packet of information special to those pumps called MySentry messages. If you have never setup this part of the pump previously, you may see a screen, called "Pump Broadcasts", at this point in the setup process.</br></br>Follow the directions on the screen. They will require you to take some manual steps on your pump to "pair" it with your Loop app.</br></br>Basically, you will need to go to your pump's main menu, scroll down to Utilities, then Connect Devices, then Other Devices, turn that setting On, and then select Find Device. Once you do that, click on the `Continue` button in Loop app and the pairing will take place. This will allow those MySentry packets of information to flow to Loop app.</br></br>This step does not apply for x22 or x15 pump users, since those pumps do not have MySentry capabilities.|

Now that your pump is paired with Loop, you should select the type of battery you are using and decide whether to use My Sentry:

1. Select your pump's battery type (lithium or alakine)
2. Leave the Preferred Data Source on Event History
1. You have your choice on enabling My Sentry (saves phone battery) vs disabling My Sentry (saves OrangeLink battery)

The Medtronic status and commands available are shown in the [Pump Setting](loop-3-medtronic.md) page.

## Modify Pump

You must first delete the old pump before you can switch to a new pump.

* If you are using Omnipod or Omnipod DASH, you must first deactivate your current pod

    * After the pod has been deactivated, a new row will show at the bottom of the pod screen
    * Tap on `Switch to other insulin delivery device` and follow the directions to complete the task

* If you are using Medtronic, scroll to the bottom of the pump screen and select `Switch to other insulin delivery device`

The [Head-Up-Display](#pump-choices) at the top of the Loop main screen will now show the add pump icon and you can [select a new pump](#add-pump).

## Time Zone

Loop allows the Pump to have a different time zone from the phone. The command to adjust time zone is found in the Pump Setting screen for an attached pump.

The schedules for the basal rates, correction ranges, insulin sensitivity factors and carb ratios stay at the pump time even if the user and their phone change time zones or when daylight savings time occurs.  To bring the pump into the same time zone as the phone, use this command in Loop. (Medtronic users - do NOT adjust time on your pump - always go through Loop.)

Select the Pump Settings display, scroll down to the Change Time Zone line, example shown in the graphic below.  You can leave the time zone offset unchanged or touch it to change to the current time zone.  Note that the 24 hour configuration pattern for basal rates, insulin sensitivity factor, carb ratio and correction range are aligned with the time zone shown on this line.

If you choose to leave the pump and phone time zones different, the pump icon on the HUD will show the clock icon to remind you.

![Command line to modify the time zone](../operation/loop-settings/img/change-time-zone.svg){width="250"}

Once the Change Time Zone command is tapped, Loop no longer shifts the 24 hour configuration pattern to the old time zone.

## Final Pump Steps

!!! warning "Please Review Detailed Pages"
    There is a lot of detailed information in the rest of this section - probably too much to absorb the first time through - although you should read it at least once.  Keep coming back while you are learning to use Loop in Open Loop.

    * [Displays](loop-3-displays.md)
    * [Settings](loop-3-settings.md)
    * [Therapy Settings](loop-3-therapy.md)
    * [RileyLink Screen](../operation/loop-settings/rileylink.md)
    * [Omnipod Common Screen](loop-3-omnipod.md)
    * [Medtronic Screen](loop-3-medtronic.md)

Now that you have paired your pump, you are ready to either add a [CGM](loop-3-cgm.md), if you have not done so, or proceed to the [Open Loop](../operation/loop/open-loop.md) page.
