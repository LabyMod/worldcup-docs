# TV Stream

The TV stream component is used to display the current active TV stream below the sign.
A custom resolution can be set to adjust the size of the stream.
The aspect ratio is always predefined by the current running stream.
If the resolution does not match the aspect ratio, black bars will be added to the top and bottom or left and right side
of the stream.

If no stream is active, the [upcoming matches](/components/matches.md) will be displayed instead with a background
image.

![stream](/.assets/stream.png)

## Configuration

The namespace and identifier in the first line is `worldcup:stream`<br>
The second line is the resolution of the stream in the format `widthxheight`<br>
If 0 is set on either width or height, the aspect ratio of the stream will be used to calculate the missing value.<br>
The resolution has a maximum of 100x56 blocks. It can also be a floating point number to adjust the aspect ratio using
the dot as a separator.

This component has the following arguments you can configure:

* `info`: Position of the current match info text. It shows the current playing team with their scores.<br>
  It has the following values:
    - `top`: The match info is displayed at the top of the stream. (Default)
    - `bottom`: The match info is displayed at the bottom of the stream.
    - `hide`: The match info is hidden.
* `fw`: Behavior of the firework attached to the stream.<br>
  These firework effects can also be placed individually on the map with
  the [effect component](/components/effect.md).<br>
  You can test the effects by manually triggering it with the `/worldcup-test` command.<br>
  The firework argument has the following values:
    - `show`: The burst and flag firework is both visible when the score increases. (Default)
    - `hide`: The entire firework is hidden for this component. (Recommended if placed individually)
    - `burst`: The burst firework shows up when the score increases for the specific team.
    - `flag`: The flag firework shows up when the score increases for the specific team.
* `off`: The offset of the canvas as a 3-dimensional vector.<br>
  The offset is relative to the sign position and can be used to adjust the position of the canvas.<br>
  The offset has the following format: `x,y,z`<br>
  The offset can be negative or positive.

### Example

Example of a TV stream component with a resolution of 16x9 blocks and the match info at the bottom.<br>
![sign](/.assets/stream_sign.png)

The stream is always rendered to the opposite side of the sign, to make it possible to hide the sign behind a block
as you can see in this example:<br>

![sign](/.assets/stream_position.png)

Example of the match info that is configured to be displayed at the bottom of the stream:<br>

![sign](/.assets/stream_match.png)