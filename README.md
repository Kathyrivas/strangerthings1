# strangerthings1

use_bpm 160
use_synth :saw
with_fx :echo do
  sample :elec_plip
  
  st_notes=[:c2,:e2,:g2,:b2,:c3,:b2,:g2,:e2]
  
  live_loop :stranger do
    index=0
    8.times do
      play st_notes[index]
      sleep 0.5
      index = index + 1
    end
  end
end
