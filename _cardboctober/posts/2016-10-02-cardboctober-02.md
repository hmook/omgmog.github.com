---
title: "02: Raycaster based look interaction"
redirect_from:
  - /post/cardboctober-02/
has_hack: true
---

For today's Cardboctober hack I'm doing some basic look interaction.

As you look at each ghost in the circle surrounding you the ghost will cover their eyes.

<!-- more -->

{% include figure.html src="2016-10/02/giphy.gif" %}{:.massive.center}

This is really basic, and uses Three's built-in `THREE.Raycaster`. You can imagine a raycaster as a laser beam shining from your eye to the point that you're looking at.

{% include figure.html src="2016-10/02/raycasting.png" %}{:.massive.center}

In this hack I'm grabbing the first object that the raycaster hits and then changing the material.
