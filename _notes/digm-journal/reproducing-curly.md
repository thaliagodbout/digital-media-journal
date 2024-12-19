---
title: "Reproducing Curly"
---
After experimenting with [[computational-sketching|Computational Sketching]], to try recreating and building upon research, we've attempted to recreate and build upon Golan Levin's Curly/[Yellowtail](http://www.flong.com/archive/projects/yellowtail/index.html) in DIGM 5010.

## Recreating Curly in Class
Before building on Curly individually, we started with collaboratively building a drawing app during class. This was the result:
<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="jOgVwYw" data-pen-title="5010 wk 3" data-user="thaliagodbout" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/thaliagodbout/pen/jOgVwYw">
  5010 wk 3</a> by Thalia (<a href="https://codepen.io/thaliagodbout">@thaliagodbout</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

While the animated lines are expressive, the lines and their paths can't be altered once the lines have been drawn. The path, speed, and form of the lines are only determined when we first draw them out.

To build upon this Curly recreation, I was interested in exploring how we could situate ourselves in this virtual space, and influence it *after* the lines are drawn and animated.

## Building Upon Curly
I wanted to be able to affect the movement of the drawn lines with my cursor. In my alteration of Curly, if the cursor intersects with the "front" of a moving line, the line stops moving across the screen and instead wriggles in place. Once the cursor moves away, the line is "released".

<p class="codepen" data-height="300" data-default-tab="js,result" data-slug-hash="wvVGBWO" data-pen-title="Curly Catching" data-user="thaliagodbout" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/thaliagodbout/pen/wvVGBWO">
  Curly Catching</a> by Thalia (<a href="https://codepen.io/thaliagodbout">@thaliagodbout</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

This sort of "catch and release" feels playful - it added some life into the virtual space, and felt like a little world of virtual worms that interact with my cursor. You can chase the worms and stop them at a particular spot on the canvas, or leave your cursor in place and let them come to you. After some time, I find they all tend to eventually end up wriggling on your cursor.

Aside from a playful worm world, this interaction lets us control when and where lines stop moving across the screen. This type of interaction might be useful if we added sound to the app - in a performance, influencing when each gesture stops and re-starts could control when a sound pauses, continues, or changes, adding more opportunities for expression.

"You created an impact from your occupancy on the screen"


### Alternative Alterations


### Pseudocode