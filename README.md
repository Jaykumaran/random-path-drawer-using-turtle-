# random-path-drawer-using-turtle-

import turtle as t
import random

timmy = t.Turtle()
screen = t.Screen()
t.colormode(255)

def random_color():
    r = random.randint(0, 255)
    g = random.randint(0, 255)
    b = random.randint(0, 255)
    color_tuple = (r, g, b)
    return color_tuple


timmy.width(15)
timmy.speed("fastest")
timmy.pensize(15)
direction = [0, 90, 180, 270]
for i in range(500):
    timmy.forward(30)
    timmy.setheading(random.choice(direction))
    timmy.color(random_color())

screen.exitonclick()

