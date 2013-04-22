# An APRS passcode generator, written entirely in JS.

-----

## Manifesto/Justification

The currently passcode hashing algorithm is a joke.  It does absolutely nothing
to prevent non-hams from injecting items into the APRS IS, and is freely
available in various implementations of open-source software, such as xastir. 

I'm tired of having to go through gyrations to generate these for people when
I help them set up APRSIS32, aprx, etc. so I wrote this.

If you're upset that this software exists, then let's work on a better way to
keep the APRS IS ham-only, rather than pretending the passcode does anything at
all to keep non-hams off of the APRS IS.

## Usage

Change the callsign between the single quotes on the
<code>&lt;body onLoad...&gt;</code> line, save, and open in a web browser.
The passcode will show up in an alert box.

This software does no checking of callsign validity whatsoever.  It _does_
however strip any SSIDs (-1, -3, -7, etc.) from a callsign if one is entered.

## License (Modified BSD license)

Copyright (c) 2013, Matthew E. Willis,
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright
  notice, this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright
  notice, this list of conditions and the following disclaimer in the
  documentation and/or other materials provided with the distribution.
* Neither the name of Matthew E. Willis nor the names of any subsequent 
  contributors may be used to endorse or promote products derived from this
  software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL MATTHEW E. WILLIS BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

-----

73 de N2PYI
