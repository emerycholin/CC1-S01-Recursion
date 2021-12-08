# CC1-S01-Recursion
import turtle

t = turtle.Turtle()
t.right(90)
t.forward(50)
t.left(180)

def draw(Blen = 75):
    if Blen < 10:
        return
    else:
        t.speed(1000)
        t.forward(Blen)
        t.right(30)
        t.color("blue")
        draw(Blen - 10)
        t.left(60)
        t.color("red")
        draw(Blen - 10)
        t.right(30)
        t.backward(Blen)
        return

draw()



