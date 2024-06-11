# Effect

The effect component is a firework spawner that creates a firework effect when a team scores a goal at the position of
the sign.<br>
You can test the effects by manually triggering it with the `/worldcup-test` command.

![effect](/.assets/effect.png)

## Effect Types

### Burst

The burst effect is a basic firework that shoots out of the component when the score increases for the specific team.
The particles have the color of the team that scored. The source position of the firework can be adjusted with the
offset argument.

![effect](/.assets/effect_burst.png)

### Flag

The flag effect is a firework that shows the flag of the team that scored in firework particles.
The position of the flag is relative to the sign position and can be adjusted with the offset argument.

![effect](/.assets/effect_flag.png)

## Configuration

The namespace and identifier in the first line is `worldcup:effect`<br>

This component has the following arguments you can configure:

* `fw`: The type of firework effect that this component should display.<br>
  The firework argument has the following values:
    - `burst`: The burst firework shows up when the score increases for the specific team.
    - `flag`: The flag firework shows up when the score increases for the specific team.
* `team`: The side of the team that the effect is bound to.<br>
  This option is only available for the burst effect. It triggers for both teams if no specific team is set.<br>
  It has the following values:
    - `left`: The burst effect is bound to the left team side.
    - `right`: The burst effect is bound to the right team side.
* `off`: The offset of the effect as a 3-dimensional vector.<br>
  The offset is relative to the sign position and can be used to adjust the position of the effect.<br>
  The offset has the following format: `x,y,z`<br>
  The offset can be negative or positive.

### Example

Example of an effect component with a burst firework effect bound to the left team side and an offset of 1.5 blocks on
the y-axis:<br>
![sign](/.assets/effect_sign.png)