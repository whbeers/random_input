# Random Input Fuzz Effect

This is a re-creation of the original Dallas Arbiter Fuzz Face effect circuit, continuing my attempts to design guitar effects using [KiCAD](https://www.kicad.org/).

The resulting design is a product of breadboarding and experimentation after an initial build of the original circuit. It emphasizes the ability to easily fine-tune the bias of each transistor to obtain a pleasant sound from a variety of NPN transistors (germanium or silicon). Besides this emphasis, it remains true to the original.

The board is built on the ["Noise Floor"](https://github.com/whbeers/noise_floor) pedal platform, which provides basic power protection, audio IO, and a footswitch with LED indicator.

![Front render](renders/front.png)
![Back render](renders/back.png)

[Schematic](hardware/RandomInput_schematic_v0.26.pdf)

Instructions for biasing transistors (using the incorporated trimpots) are provided in the schematic. (This was the approach that worked for me, after a few hours of research. I'm by no means an expert and would welcome feedback.)

## Credit
The basic schematic I worked from is widely available on the internet. At the same time my research drew on analyses from far-greater experts than myself, as well as published circuit diagrams. Most notably:
 - [CODA Effects' circuit analysis](https://www.coda-effects.com/p/circuit-analysis-fuzz-face.html)
 - [RG Keen's analysis](http://www.geofex.com/article_folders/fuzzface/fffram.htm)
 - [PedalPCB Twin Face](https://www.pedalpcb.com/product/twinface/)

## Versioning

My pcb designs utilize the following versioning scheme (I'll add to this as I produce more revisions):
 - v0.0XX: A candidate design that has not yet been produced and tested.
 - v0.XX: A design that has been produced, tested, and any initial errors addressed.

The current version of the Random Input Fuzz effect is v0.26.

## Planned TODOs before v0.30
 - Re-place and re-route lower connector to top of board, in alignment to the approach I've taken with the [Noise Floor](https://github.com/whbeers/noise_floor) utility board. [DONE in v0.25!]
 - Later, migrate indicator LED and power protection circuit to Noise Floor. [DONE in v0.25!]
 - Fix any issues I identify in testing produced v0.2 boards

## Name
*The name "Random Input" is a reflection of the nature of the effect (a very basic fuzz) and security nerdery (fuzzing software using random input being a primitive technique to surface errors).*
