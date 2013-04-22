* APRS passcode generator, entirely in JS.

*** Manifesto

The algorithm is a joke, does absolutely nothing to prevent non-hams from
connecting to the APRS IS, and is freely available in various implementations
of open-source software, such as xastir. 

I'm tired of having to go through gyrations to generate these for people when
I help them set up APRSIS32, aprx, etc.

If you're upset that this software exists, then let's work on a better way to
keep the APRS IS ham-only, rather than pretending the issue doesn't actually
exist.

*** Usage

Change the callsign between the single quotes on the <body onLoad...> line,
save, and open in a web browser.  The passcode will show up in an alert box.

This software does no checking of callsign validity whatsoever.  It _does_
however strip any SSIDs (-1, -3, -7, etc.) from a callsign if one is entered.

73
N2PYI
