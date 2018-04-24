![alt-text](https://github.com/iwoplaza/Coffi/raw/master/Misc/banner-lowres.png "Banner")

# Coffi
This project is an Audio Plug-in realised using the JUCE framework, mainly exported as a VST plug-in. It's a simple in look granulator-esque synth that is advanced under the hood. It was started in February of 2018.

## What does it do?
As of writing this, it can create interesting patterns and ambiences using what's called "grains". A single grain isn't very special, it can playback a sample loaded into the synth by the user at a specified place, with a pitch and pan. The strength though comes with numbers. You can have up to **50** grains playing at once, each at a different place, a different pitch and pan.

## What can I do with it?
The first thing that comes to mind, is pads. You can create pads out of pretty much any sample. However, turning down knobs like *spread*, *stereo*, *displace* and *detune* to an absolute 0 and leaving the *delay* knob at a bare minimum just above 0, you can get some really great resonant sounds.

## Controllers
To automate the innerworkings of the synth, controllers were created. You have 6 controllers at your disposal:
 - a Synth ADSR envelope - this is your plain-old-simple Attack/Decay/Sustain/Release envelope, which is used to control the gain of the whole synth.
 - a Grain ADS envelope - this is a variantion on the ADSR setup, since it only has Attack/Decay/Sustain, removing Release from the equation. This envelope is used to control the gain of each individual grain through it's lifetime.
 - 4 custom controllers - these are user-created controllers that can be drawn inside the UI, and aren't used internally.
 Each of these 6 controllers can, additionally to their original use, be linked (routed) into most of the synth's parameters.
