---
title: Computational Sketching
created: 2024-09-19
last_modified_at: 2024-12-19
---

<div class="overview">
Explorations in Computational Sketching through 2D drawing.
</div>

In Week 1 of Foundations of Digital Media, we talked about [John Maeda](https://en.wikipedia.org/wiki/John_Maeda)'s explorations in interactive graphics in combining computation with traditional art techniques.

A few key takeaways from [Graham's Week 1 notes on computational sketching](https://alicelab.world/digm5010/#computational-sketching):
- "the most **interesting** pixels on the screen are the mouse"
- "the mouse represents not just **space** but also **time** -- use it"

This goes back to our discussion about [[what-makes-something-interesting|what makes something interesting]]. These most interesting pixels that Maeda talks about represent **you** in the digital space - this could be the cursor of your pointing device, or perhaps your focus indicator. It situates you in a digital environment, and it's your gateway to interacting with elements in this environment.

## Learning about 2D drawing in class
While I've used [p5.js](https://p5js.org/) in the past (and I love it), I'd never really used JavaScript's Canvas API directly.

Following along with Graham in class (and slightly modifying his example), I made a quick sketch that creates [[pseudorandomness|random]] colourful threads when you move the cursor. Clicking the canvas wipes it clean.
<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="ExBJXyx" data-pen-title="Untitled" data-user="thaliagodbout" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/thaliagodbout/pen/ExBJXyx">
  Untitled</a> by Thalia (<a href="https://codepen.io/thaliagodbout">@thaliagodbout</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

It reminds me of my colourful piles of thread cuttings that keep growing - I don't know why I hang onto those but I do think they're pretty.

## Representing Time in a Gesture
Next is to create a canvas that allows us to draw in response to mouse/touch movements. I also want to think about how to represent **time** in a gesture - how can we represent time in a drawn gesture?

Let's start out with a very simple drawing app. I made this one to start with as a base.

<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="VwoZJxO" data-pen-title="Simple Draw" data-user="thaliagodbout" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/thaliagodbout/pen/VwoZJxO">
  Simple Draw</a> by Thalia (<a href="https://codepen.io/thaliagodbout">@thaliagodbout</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

Reminiscent of writing with a fountain pen using thin ink on absorbent paper, I tracked the speed of the cursor to create thick, inky blotches whenever you move at a slower speed. (I actually meant to make this a smoother transition from thick to thin line widths, but ended up liking the sudden inky blotches.)

<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="mdNddYJ" data-pen-title="Simple Draw - inky" data-user="thaliagodbout" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/thaliagodbout/pen/mdNddYJ">
  Simple Draw - inky</a> by Thalia (<a href="https://codepen.io/thaliagodbout">@thaliagodbout</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<img alt="Curving scribbly lines with black inky blotches at curve joints" src="{{site.baseurl}}/assets/inkyblotches.png">

Other ideas for ways to map time in a gesture:
- Having the width of a line "pulse" on intervals
- "Echoes" of a line appearing after a length of time depending on the speed of the gesture

These two only create static lines, but next we'll be animating the lines to give them some more life. We do this in [[reproducing-curly|Reproducing Curly]]!