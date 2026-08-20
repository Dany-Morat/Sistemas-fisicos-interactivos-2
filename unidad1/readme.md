


``` js
const { visualid } = createParams('visualid')

setcpm (15)
let drum= stack (
  s("bd").beat("0,2,8,12",16),
  s("hh").beat("0,2,4,6,8,10,12,14",16),
  s("cp").beat("4,12",16),
  s("oh").beat("7, 15",16), 
). bank("RolandTr909"). visualid("drum")
$drum: stack (drum, drum.osc())

let bass = note("[c2 c2 g1 a1]"). sound("sawtooth"). visualid("bass")

$bass: stack (bass, bass.osc())

 let melody= note("[c4 e4 g4 a4 g4 e4 d4 c4]"). sound("supersaw"). visualid("melody")

$melody: stack (melody, melody.osc())

```
