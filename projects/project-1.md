---
layout: project
type: project
image: images/micromouse.jpg
title: Air Hockey
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2017-12-04
labels:
  - EZ Java
  - Java
summary: For the final group project in ICS111, we created an air hockey simulation.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

Our Air Hockey project is a 2-player game constructed using Java and the library EZ Java. Played on one computer, where each player has control over an individual puck's direction in going up, left, down, or right with either the WASD or IJKL keys. Upon getting past the instruction screen, users will be greeted with a rectangular rink and a puck with a starting velocity. The game is won once a player "scores" 7 times by hitting the puck with their paddle into the opposing player's goal.

In this project, I was in charge of the puck class, while my other team members were in charge of the paddle and goal post classes. My work involved keeping the puck moving and the behavior of the puck upon collision with other objects, including the wall, goal area, and paddles.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



