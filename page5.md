# INFOTC 1000 Final Project
## Page 5

![Autumn Banner](https://www.pngkit.com/png/detail/426-4265210_huge-fall-sale-banner-autumn-leaves.png)

As this semester comes to a close, I wanna say thanks for such a *great* semester! I've learned a **lot**, and I've enjoyed learning new things about IT.
Can't wait to see what the future holds!

I was a little nervous when I decided to switch from Bio to IT, but I'm glad I did!

![Code Picture](codepic.png)

I'm excited to learn all sorts of new things in the coming semesters, including:
- More programming
- More media design
- and more, and more IT stuff!

---

Here's my final code snippet for this project!

```
#recursion and turtle graphics

#this program draws a Turtle Graphic using recursive functions

import random
from turtle import Turtle

SPEED = 0

#recursive function
def recursive_circles(turtle, angle, quantity, delta, radius):
    colors = ["orange", "violet", "turquoise"]
    color = random.choice(colors)
    width = random.randrange(1, 5)
    turtle.color(color)
    turtle.width(width)
    turtle.left(angle)
    turtle.forward(delta)
    unit_angle = 360.0/quantity

    for x in range(quantity):
        turtle.circle(radius)
        turtle.right(unit_angle)
    radius = radius - delta
    if (radius > 1):
        recursive_circles(turtle, angle, quantity, delta, radius)
        

#main function
def main():
    teddy = Turtle()
    teddy.speed(SPEED)
    recursive_circles(teddy, 2, 2, 1, 200)

main()
```
---

Navigate between pages:
- [Page One](page1.md)
- [Page Two](page2.md)
- [Page Three](page3.md)
- [Page Four](page4.md)
- Page Five



