##Turtle Graphic Code

```
import random
from turtle import Turtle

def Recursion(turtle, sides, length):
    colors = ["red", "black", "pink", "green", "blue", "purple", "orange"]
    Random_Color = random.choice(colors)
    turtle.color(Random_Color)
    turtle.right(360/sides)
    turtle.forward(length)
    length = length - 1  
    if (length > 5):
        Recursion(turtle, sides, length)
def main(): 
    animation_speed = 0
    Peter = Turtle()
    Peter.speed(animation_speed)
    Recursion(Peter, 5 , 150)

main()


```
