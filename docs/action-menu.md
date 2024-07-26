# Action Menu

![action-menu](~/images/action-menu.png)

Used to add controls to your avatar which are accessable through the VRChat Action Menu.  
  
## Controls

# [Toggle](#tab/toggle)
## Toggle

A control which can be toggled ON/OFF.  
![toggle](~/images/action-menu-toggle.png)

- **Group:** Specifies which group the toggle belongs to, you can use any string to represent a group. When grouped, only one toggle turned ON at a time.
	- **Default:** Which toggle is ON by default for the group.
	- **Off State:** Which toggle represents the OFF state for the group.  This toggle turns ON when other the other grouped toggles are turned OFF.
- **Default On:** When enabled the toggle will start ON
- **Parameter:** The parameter used for this control.  If left blank, or the parameter name does not exist, one will be auto-generated.
- **Fade In:** Time in seconds for the control to fade in.
- **Fade Out:** Time in seconds for the control to fade out.
- **Hold:** Time in seconds the control will stay ON before fading out.  For example, you may want an animation to play for minimum of X seconds even if the user has turned the control OFF.

# [Button](#tab/button)
## Button

A control which can be temporarily ON/OFF.
![button](~/images/action-menu-button.png)  

- **Parameter:** The parameter used for this control.  If left blank, or the parameter name does not exist, one will be auto-generated.
- **Fade In:** Time in seconds for the control to fade in.
- **Fade Out:** Time in seconds for the control to fade out.
- **Hold:** Time in seconds the control will stay ON before fading out.  For example, you may want an animation to play for minimum of X seconds even if the user has turned the control OFF.

# [Slider](#tab/slider)
## Slider

A control which can set a value between 0% and 100%.
![slider](~/images/action-menu-slider.png)

- **Animation:** An animation clip applied to the FX layer. The control value determines where the animation is sampled between it's start and end frames.  Unlike most animations it does not update over time.  For example, if the control is set to 50% then values will be applied from the middle of the animation.  This means you must supply an animation with at least two keyframes.
- **Default Value:** The default value for the control.
- **Parameter:** The parameter used for this control.  If left blank, or the parameter name does not exist, one will be auto-generated.

# [Sub Menu](#tab/submenu)
## SubMenu
Defines another menu for additional controls.  Click the **Sub-Menu** button to view/edit those controls.  
![sub-menu](~/images/action-menu-sub-menu.png)  

---

## Options
Options determine what happens when using a control.  [Learn about Options.](action-options.md)  