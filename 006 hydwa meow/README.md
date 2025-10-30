# hi you already know what time it is

# hydra patch documentation

## i want to be able to do something cool like a fake puddle of water
#### this is a problem i only keep looking at my screen and not actually documenting anything lol

#### i started with a voronoi function, turned the brightness down to get a wave of little stars in the air !

#### hit them with the luma but i wonder if i can make it blurry, also i love the modulate repeat x function too 

#### .thresh().blend(o0,1) has been fun for feedback


``` // Type some code on a new line (such as "osc().out()"), and press CTRL+shift+enter
voronoi(20,2,12).color(4,2,0).brightness(1).thresh().mask(shape(10))
  .scale(1,0.5,0.05)
  .out(o0)```
  
# YAY it works !