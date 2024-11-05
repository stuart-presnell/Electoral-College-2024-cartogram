# Electoral College Cartogram 2024

A map of the US in which each state is scaled 
to represent its number of Electoral College votes 
in the 2024 presidential election. 1 square = 1 EC vote.
Edit the results file and recompile to update the map as results come in.

* States in which the D/R candidate is favored are colored light blue/pink.
* Tossup states are colored gray. 
* States won by D/R are colored blue and red.

**New for 2024**: Splitting EC votes in Nebraska and Maine 

**New for 2024**: Bar chart of EC votes won or expected by each candidate 
at the top of the map. 
Each column of 2 squares corresponds to 15 EC votes.


## How to use this

Compile `main.tex` to generate and update the map.
By default this inputs `2024-results.tex`, 
which is where the current results and expectations are stored.

The file `2024-results.tex` contains a line for each state 
(and each district for Nebraska and Maine).
As results come in, edit the entry for a state 
and then recompile to update the map.
The styles (defined in `main.tex`) are:
* `Dfav`: D candidate is favored to win — light blue
* `Rfav`: R candidate is favored to win — light pink
* `Dwin`: D candidate has won — dark blue
* `Rwin`: R candidate has won — dark red
* `toss`: The race is a tossup — light gray

At the bottom of `2024-results.tex`
we define four variables:
`Dfavcount`, 
`Rfavcount`, 
`Dwincount`, and
`Rwincount`.
These control the bar chart at the top of the map. 
The value of each variable is the number of EC votes won or expected for each candidate.
Unfortunately I haven't figured out 
how to compute these automatically from the results data,
so you'll have to update these numbers by hand as results come in.
(Maybe I'll get this working for 2028!)

The commands that define how to draw the map and the bar chart 
are in 
`draw-states.tex`
and
`EC-bar.tex`, 
but you don't need to edit anything in these files.

## Contact

* Bluesky: [@logopetria.bsky.social](https://bsky.app/profile/logopetria.bsky.social)
* Twitter: [@logopetria](https://x.com/logopetria)
* Mastodon: [@logopetria@mastodon.social](https://mastodon.social/@logopetria)

