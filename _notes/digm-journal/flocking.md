---
title: Building Boids
created: 2024-10-30
last_modified_at: 2024-11-14
---

<div class="overview">
Documentation and reflections on building boids together in class.
</div>

After discussing research around [[steering-behaviours|steering behaviours]], we dove into more explorations in [[reproducing-research|reproducing research]].

## Progress in Week 7 Class

We worked on reproducing Craig Reynolds' boid steering behaviours and created this sketch together in class:

<p class="codepen" data-height="500" data-default-tab="html,result" data-slug-hash="VworXVj" data-pen-title="5010 wk 7" data-preview="true" data-user="grrrwaaa" style="height: 500px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/grrrwaaa/pen/VworXVj">
  5010 wk 7</a> by Graham (<a href="https://codepen.io/grrrwaaa">@grrrwaaa</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

For this sketch, we programmed the boids to gravitate towards the cursor (and away from the cursor when clicking with the mouse) using flow fields.

## Progress in Week 8 Class

To continue building on last week's sketch, we further explored flow fields and implemented the behaviours described in Reynolds' paper:

- Separation (avoidance)
- Cohesion (center)
- Alignment

This created boids that exhibited natural flocking behaviours, combining simple instructions to generate complex-seeming behaviours. We spent a lot of time tweaking the different parameters to create believable steering behaviours (and this showed how much Reynolds must have done so as well when creating algorithms for these behaviours). We've been growing our own little [[microworlds|microworld]] :)

Here's Graham's codepen that we worked on collaboratively during class:

<p class="codepen" data-height="500" data-default-tab="html,result" data-slug-hash="KKOGLqW" data-pen-title="5010 wk 8" data-preview="true" data-user="grrrwaaa" style="height: 500px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
  <span>See the Pen <a href="https://codepen.io/grrrwaaa/pen/KKOGLqW">
  5010 wk 8</a> by Graham (<a href="https://codepen.io/grrrwaaa">@grrrwaaa</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

## Future modifications to our boids microworld

I didn't have time to continue building upon our boids recreation from class, but considered these modifications:

- What could happen when the boids collide?
    - Do they disappear?
    - Maybe they eat each other and one grows bigger???
    - Maybe they reproduce and create more boids?????
    - Do boids have a lifespan?
- Could we situate ourselves in this virtual boid world in a more long-lasting way?
    - Could we place currents using the cursor that affect the flow fields? Maybe this affects the direction and speed of the boids?
	- Could we place obstacles that the boids must avoid?