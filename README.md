import turtle

def draw_flower(t, petals):
    for i in range(petals):
        # Draw a petal
        t.forward(100)
        t.right(360 / petals)

    # Move to the next flower
    t.up()
    t.forward(120)
    t.down()

# Create a TurtleScreen and Turtle
screen = turtle.Screen()
t = turtle.Turtle()

# Set up the starting position and orientation
t.left(90)

# Draw some flowers
for _ in range(3):
    draw_flower(t, 20)

# Hide the turtle
t.hideturtle()

# Exit the app when the user closes the window
screen.exitonclick()
