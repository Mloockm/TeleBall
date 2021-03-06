TeleBall - Version 1.4 - 04/22/19
---------------------------------

Improved documentation and website: Updated outdated links and increased
the font size to fit better to 2019 website styles.

TeleBall - Version 1.3 - 06/03/16
---------------------------------

Improved documentation: Updated the Bill of Material (BOM) in the
"Electronics" section (some links and some part numbers where outdated).

From a technical perspective, Version 1.3 is identical to Version 1.2.

TeleBall - Version 1.2 - 01/01/15
---------------------------------

* Change: The brightness adjustment has been moved to the advanced
  configuration mode, as usage tests showed that it is far less often used
  than the speed adjustment, and therefore it started to annoy soon.

* Change: Advanced menu: If you set the leftmost paddle position identically
  to the rightmost paddle position, then no paddle change is assumed. The
  idea is to be able to skip quickly through this menu setting without the
  necessity to set the paddle position each time.

* Change: The minimum speed is now faster (500ms instead of 600ms delay per
  pixel) and the maximum speed is now also faster (50ms instead of 75ms).

* Bugfix: The "X" in the EEPROM menu was not always accessible.

* Bugfix: You were not able to catch a ball that was already one line above
  the paddle and THEN you moved the paddle below it - even if you were fast
  enough that you should have catched this ball. 

* Bugfix: With a speedy paddle movement you could influence the ball even if
  the ball was far away from the paddle.

* Bugfix: Sometimes when adjusting the speed and the controller wheel was at
  the very left position, you saw no pixels illuminated while exactly one
  should have.

* Bugfix: The EEPROM fingerprint was not written on new devices, which means
  that new devices did not remember any settings, i.e. the EEPROM feature was
  broken there.

* Bugfix: The advanced menu already opened after a ~1sec button press instead
  after a ~4sec button press.

* Bugfix: Tennis: The pairing of two devices did not work, when one was in the
  won or lost state of BreakOut, while the other one was powered on. There
  were also some other states that prevented pairing, so this should be rock
  solid now.

* Bugfix: Tennis: When one of the players suddenly switched off his device or
  walked out of the radio range (or similar events), then the other device was
  left in an undefined state. Now it goes back to BreakOut.

* Bugfix: Tennis: Sometimes the won or lost smiley stayed visible, on the
  slave's screen when the master device was resetting the match.

* Bugfix: Tennis: If the game speed was set on the slave device, then when
  leaving the configuration menu, there was no short game pause and the ball's
  position and direction was random, which sometimes lead to weird results
  like left/right bouncing balls.

* Bugfix: Tennis: If during pairing a player pressed the button while waiting
  for the other player to join, the device went into an undefined state.

* Bugfix: Tennis: If during pairing a player pressed the button immediatelly,
  i.e. if he did not wait for the initial "?" to disappear, unwanted effects
  could occur.

* Bugfix: Tennis: When the slave device was the last to acknowledge to play
  tennis, then there was no delay, before the game started.

* Bugfix: Tennis: When the configuration menu was entered while the ball was
  still in pause mode (e.g. directly after a lost ball), then when leaving
  the configuration menu lead to a freezing ball, i.e. it did not start moving
  again at all; you needed to reset the match.

* Optimization: Saved SRAM by moving constant lookup-tables to PROGMEM.

TeleBall - Version 1.1 - 12/24/14

* Bugfix: BreakOut: When solving the game, i.e. when the third level is
  successfully mastered, the applause sound is played and the smiley face
  is shown.

* EEPROM: The device is now able to permanently store user preferences. For
  doing so, enter the advanced config menu by pressing the button 4 seconds
  while being in the standard menu. After configuring the paddle, you can now
  choose "square" for saving your preferences or "X" to revert back to the
  factory default values.

TeleBall - Version 1.0 - 12/21/14

* First release on final TeleBall hardware

TeleBall - Version 0.1 - 8/3/14

* The very first version of TeleBall was developed on the Arduino experimentor
  platform DuinoKit: http://duinokit.com/ShowAndTell/viewtopic.php?f=4&t=14



Last modified by sy2002 on 3rd of January 2015