# Castle-Greyscale-ep0
A .dat programming adventure

Castle Greyscale is an adventure-themed programming challenge that you "play" by writing code to decipher the contents of a binary .dat file.

How to "play": 

The challenge is made up entirely of the contents of the .dat file. Combine the information in this document with whatever human readable text you can find in the .dat. Then write code in your preferred language to work out the data format and learn about the game.

Unlike typical programming challenges, the goal is NOT to write a one-shot program that solves a problem and generates some verifiable output, and there are no leaderboards. Instead, code should be employed as a tool to probe and explore the contents of the file. This doesn't necessarily have to involve a single monolithic program. You may for example write one program to probe the file format, and another to parse and navigate the file. You may even employ pen and paper for certain aspects. It all comes down to preference.

.dat Format:

* Observing the information below is part of the intended challenge, and I don't know if it's realistic to solve without doing so.

* The .dat contains some human readable text. These are intentional breadcrumbs to help you in your adventure.

* There are no INTENTIONAL "gotchas" or subtle word tricks. But, since we're talking about parsing, details are critical.

* Data formats for a particular type are consistent throughout the file - once you work something out there are no rug-pulls. However later objects of a particular type may contain additional sub-objects that require additional probing and parsing. 

* All strings are prefixed with a uint16 size.
* Some strings are empty but still present.

* Object arrays are prefixed with a uint8 count followed by the object/s back to back.
* Some arrays are empty but still present.

* Except as described above, numerical values are always uint32.

* Most strings are obfuscated using a simple XOR CIPHER with the LOWER 8 BITS OF A UINT32 in order to facilitate a sense of progression. I recommend against trying to decipher all of the obfuscated text before "exploring", but play your way.

* Much of the file data is there for you, not your program.

* There are no "magic number" puzzles or logic required - all required data (but not necessarily skill) is presented in this file and the .dat.

* Hints and discussion are encouraged, but please mark and obfuscate any spoilers.

* Feedback is welcome.
