# List of Upcoming Matches

This component displays a list of upcoming matches. The list is updated automatically and shows the next matches that
are scheduled to be played.
The length and size of the list can be configured by using the dimension option.

![matches](/.assets/matches.png)

## Configuration

The namespace and identifier in the first line is `worldcup:matches`<br>
The second line is the dimension of the list in the format `widthxheight`<br>
The dimension has a maximum of 100x56 blocks.

The width determines the size of the text and the height the number of matches that are displayed.

### Example

Example of a matches component with a dimension of 5x6 blocks.<br>
![sign](/.assets/matches_sign.png)

The list is always rendered to the opposite side of the sign,
to make it possible to hide the sign behind a block as you can see in this example:<br>

![sign](/.assets/matches_position.png)