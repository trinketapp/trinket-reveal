---
layout: slide
title: 
lang: Python
data:
  background: "#69b3ef"
---

<section markdown="1">

##  {{ page.lang }}

I think [Python is the best first language](http://blog.trinket.io/why-python){: .external}

To see {{ page.lang }} examples, press the down arrow:

[![Down arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png)](#/2/1){: .image .navigate-down}

</section>
<section markdown="1">
Python's built-in `turtle` module is a great visual intro to coding that students can easily `Play` with: 

{% include trinket-open type='python' %}
import turtle

tina = turtle.Turtle()

for c in ['red', 'green', 'yellow', 'blue']:
    tina.color(c)
    tina.forward(75)
    tina.left(90)

tina.penup()
tina.backward(100)
tina.write("Hello world!")
{% include trinket-close %}

</section>
<section markdown="1">

Python is also a powerful for `Showing` how to get insights from data.  Check out this basic `matplotlib` graph by Gil Forsyth:

{% include trinket-open type='python' height='600' width='100%' %}
import numpy #can't forget this!
import matplotlib.pyplot as plt #our shortcut

x = numpy.linspace(0,5,20)      #create our first array
y = x**2    #this is how Python does exponents

plt.plot(x,y,'*')           #create the plot
plt.show()                  #show the plot
{% include trinket-close %}

</section>
<section markdown="1">

## What's Next? The Web!

Press the right arrow to move on to HTML.

[![Up arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png){: style="transform: rotate(270deg);-webkit-transform: rotate(270deg);"}](#/3)

</section>