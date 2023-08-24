# Notes for WindySynth's fork of NuEVI code
The reason for this fork of NuEVI was to experiment with different fingerings for the NuRAD and add some other features.

## NuRAD XVI and XVR fingering
XVI and XVR are the same as EVI and EVR respectively, except for the following changes:
   * Lifting LH2 increases note value by 4 semitones
   * Lifting LH3 increases note value by 3 semitones
   * Pressing LHp1 increases note value by 1 semitone
   * Pressing RHp1 increases note value by 1 semitone
   * Pressing LHp2 decreases note value by 1 semitone
   * Pressing RHp2 decreases note value by 2 semitone

By changing LH2 and LH3 this way LH1 LH2 and LH3 are sort of the embouchure. 
Neither LHp3 or LHs were changed, so they can still be programmed as before in the menus.
I have mine programmed so LHp3 decreases by 7 semitones and LHs increases by 3 semitones.
This way the almost the entire range of a trumpet can be reached witout changing roller positions.
Also, any not fingered with the right hand can easily be arpegiated by lifting LH2 then LH3 or vice versa. 

## NuEVI XVI and XVR fingering (ver >= 1w6s6)
    * K1 and K5 at the same time decreases note by 2 additional semitones
    * K2 and K6 at the same time decreases note by 1 additional semitone
    * K3 and K7 at the same time decreases note by 3 additional semitones

So, for exmample, if you are already holding K1 down, you can slide your 
finger and touch the K5 trill key and go down 2 more semitones. 


## Gliss(ando) BITE CLT/GLS menu additions.
Set SETUP CTL/BITE CTL to GLS
Then in SETUP CTL/GLISS set the rate between notes in mS (0 mS for off).
Then use the bit sensor sets step size (1-4).
When not biting, there is no glissando effect. Changing the amount of bite changes the step size.
Then just play legato between two notes and it plays the notes at the interval until reaching the 2nd note.
If a step is large enough that it would step over the target note, it just steps by 1 until reaching the target.
If you change amount during the run, the step size changes. If you release the bite all the way,
the note goes to the target note immediately.
If you change notes (still legato) before reaching the 2nd note, it starts going toward the new target.

## Version Numbering
I got the 1.5b9 version from Johan because that was in the NuRAD I purchased and wanted to start there.
I'm not sure what was intended in the numbering scheme for the NuEVI project, but I started with 1.5b9 and I was just going to increase it to 1.5b10 but that string didn't fit on the screen, so I just change to 1.5c1.
Also, when i added 1.5b9 to the forked repo I couldn't figure out how to add the simulation/imgui sub project, so this fork doesn't include that.

In March 2023 I re-forked 1.6.0.  For my changes, I'll change the '.' like this 1w6s3 
