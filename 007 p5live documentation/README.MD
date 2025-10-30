# today i worked with my good friends maria and zoe and we made a lot of fun visuals using p5.live and the hydra library that was inside of it !!

### a lot of the inital findings were essentially starting with a voronoi (the classic) and running everything through so many different effects until we found something that we liked. 

### on top of that, zoe 🥹 and maria 🥺 were very helpful and super cooperative in the visual process. great back and forth was had when it came to debugging a lot of the things that would act up. ESPECIALLY THIS ONE. 

```.add(solid(.2,0,.3)).mask(shape([20,5]).scale([1,2,3]).repeat(5,5)
.rotate(1.5)).scrollX([0.1,-0.0625,0.005,0.00001],0)```

### THIS EVIL LINE kept breaking on us until we had to realize that we had forgotten some of our syntax. OOPSIES.

### everything else kind of ran through a bus of some sort, but we ended up commenting out a lot of the effects because it just looked like vomit at the end of the day. check it. here's the whole patch.

```// https://orangemilkrecords.bandcamp.com/track/hikari


let libs = ['https://unpkg.com/hydra-synth', 'includes/libs/hydra-synth.js']
let hydra = new Hydra()
hydra.setResolution(window.innerWidth*2, window.innerHeight*2) // retina res

// here lol

bpm = 120
voronoi(7,2,1)
  .scale(() => Math.sin(time)+1*2)
  .repeat(() => Math.sin(time)*10)
.modulate(noise(6),.22)
//.diff(o0)
.modulate(noise())
.add(gradient(1,1))
//.thresh()
.colorama([1,2])
	.rotate(1,1)
//.modulatePixelate(noise(25,0.5),100)
//.diff(o0)
.modulateScale(osc(3,0.5),-0.5)
.mask(shape(([3,5]))
.scale(3))
.repeat(40,40)
.kaleid([5,50])
//.luma(0.5,0.1)
.invert([0,1])
.scroll(0.1,-0.3)
.rotate()
.add(o0,0.5)


  .modulateRotate(o0)
  .scale(() => Math.sin(time)+1 *1.5)
  .modulate(noise(2,2))
  .rotate(1, .2)
  .modulate(noise(4))
  .add(gradient())



.add(solid(.2,0,.3)).mask(shape([20,5]).scale([1,2,3]).repeat(5,5)
.rotate(1.5)).scrollX([0.1,-0.0625,0.005,0.00001],0)

.out(o0)








// ends here```

### shoutout foodman ! he was the backing track to a lot of our work 🦍 and using the bpm function ended up being so clutch because it really fit the music! 

### i learned today that i didn't really like the gradient option as much as i thought i would because the zero'd in settings make it look red and green. YUCKY. 

#### today's mvps were .modulate(noise) and .mask(shape) -- if no one has me i know those two have me !