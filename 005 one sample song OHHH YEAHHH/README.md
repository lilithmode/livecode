# what's up fellas we used the SCRUB OPTION
```setcpm(80/4)
$: s("processed:1").scrub("{0.1!2 .25@3 0.7!2 <0.8:1.5>}%8").slow(0.50).gain(0.2).phaser("<8>").orbit(1)
//werk

$: s("processed:1").scrub("{0.1!4}%6")
  .slow(0.5).gain(0.1).pan("<1 .5 2 0>")
  .room(0.5).rlp(10000).rfade(0.5)
//triplet vibe

$: s("processed:1").scrub("{0.3!4}%2")
  .fastGap(2).gain(0.3).pan("<.5 1 .5 0>")
//weird pan

$: s("processed:1").scrub("{0.7}!2").crush("5").delay(.25).delayfeedback("<.25 .5 .75 1>").gain(0.8)

$: s("processed:1").scrub("{0.1}")
  .struct("x ~ ~ x ~ x x x ~ x ~ x ~ ~")
  .slow(0.5).speed(1).gain(0.2).orbit(1)
//weird ass snare

$: s("processed:1").scrub("{0.12}").slow(0.1)
  .struct("x ~ x ~").duckorbit("1:2").duckattack(0.0).duckdepth(1)
//weird ass kick
  .slow(0.5).speed(.5).penv(36).pdecay(.23).decay(2).distort("1").gain(0.5)
 ```
 
### ok it wasn't that bad. to be quite honest i just checked the repository for strudel and messed around. no bugs ! i think i get strudel now hehe :3c 

### full sample included in the folder <3 shoutout dottovu