# design-patterns
Study design patterns

The Observer Pattern

In working on a CV project, I came across the concept of the Observer Pattern, in which one object can notify another
when its state changes. While reading frames from a camera in order to perform computer vision tasks, the basic examples
are reading every frame and performing analysis on every frame.  I would like to let lighter weight analysis happen on
every frame.  When a change is detected, then start a more expensive analysis. In order to test this. I have created "input-loop.py"
that mimicks my camera input. It runs in an infinite loop, flips a coin (generates a random integer between 0 and 1), and waits
for 1 second so that I can see what is happening.

The goal is to get my observer to notify my only when the flip moves from 0 to 1 or 1 to 0.