This is a KiCad project for a clone of PAiA's discontinued midi2cv8 V/Hz daughterboard.  It was designed from the same schematic as the original and is being shared with you under the kind permission of PAiA.  When installed, the board looks like this:

![image](http://i.imgur.com/L88IYDK.jpg)

At the moment, there are [three bugs](https://github.com/synthead/midi2cv8_vhz_daughterboard/issues) in the circuit design.  I am only going to build one of these things, so it's unlikely that I'll fix them, so I figured that I would leave a note about it here.  These three bugs are solved by adding the wires below and bridging pin 8 of the 4051 to ground with a blob of solder.  The workarounds, when in-place, look like this:

![image](https://cloud.githubusercontent.com/assets/820984/19833827/5a52c408-9e05-11e6-9223-d5be5d4695d1.png)

In addition, if you're adding this V/Hz daughterboard to a midi2cv8 that is already configured for V/octave CV, you'll have to change two resistors on the midi2cv8 motherboard.  This wasn't obvious to me and spent a couple days trying to figure it out, so I thought I'd mention it here as well.  Here are the values from page 12 of the midi2cv8 manual:

|Designation|Value|Color Code A-B-C|
|---|---|---|
|\*R28|2700|red-violet-red|
|\*#R32|2700|red-violet-red|

Also, if this is the first time you're etching a board, I highly recommend tearing out a glossy page from a magazine and printing onto it for your toner transfer.  Also, don't bother with clothing irons.  I use an unmodified Swingline 1000L laminator.  Tape up the magazine paper so it doesn't slip around, then run it through the laminator a dozen times or so.  If you do it right, you'll end up with a transfer looking like this:

![image](http://i.imgur.com/YUtfN5u.jpg)

To get a head start, rendered PDFs for the PCB and the silk screen can be found in [the `rendered/` directory](https://github.com/synthead/midi2cv8_vhz_daughterboard/tree/master/rendered).  If you fancy it, you can transfer toner from the silkscreen PDF to the front of a single-layer PCB for a poor man's silkscreen.  It actually works really good and looks really nice!

Enjoy!
