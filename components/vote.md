# Vote Station

Before a match starts, players can vote for the team they think will win the match using this voting station.
At the end of the match, the voting results will be displayed on all voting stations.

A voting station is bound to a specific team side (Left or right) that can be configured in the component text.

![vote](/.assets/vote.png)

## Configuration

The namespace and identifier in the first line is `worldcup:vote`<br>
The second line is the size of the flag in the format `widthxheight`<br>

This component has the following arguments you can configure:

* `team`: The side of the team that the voting station is bound to.<br>
  It has the following values:
    - `left`: The voting station is bound to the left team side.
    - `right`: The voting station is bound to the right team side.
* `off`: The offset of the flag as a 3-dimensional vector.<br>
  The offset is relative to the sign position and can be used to adjust the position of the voting station.<br>
  The offset has the following format: `x,y,z`<br>
  The offset can be negative or positive.

### Example

Example of a voting station component with a flag size of 3x2 blocks and bound to the left team side.<br>

![sign](/.assets/vote_sign.png)

The voting station is always rendered above the sign, to make it possible to hide the sign under a block as you can see in this example.<br>
Note that the flag has an offset of -1.5 blocks on the y-axis to fit it on the image.<br>

![sign](/.assets/vote_position.png)