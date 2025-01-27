SamplerBox
==========

SamplerBox is a pocket-sized sound module based on `Raspberry Pi <https://www.raspberrypi.org/>`_ for use with MIDI devices in your bedroom, studio, or on the stage.
It is completely open-source which means it is forever evolving, making it a formidable alternative to other commercial MIDI samplers and expanders on the market.

.. image:: http://samplerbox.readthedocs.io/en/latest/_images/SamplerBoxPlayer.jpg


How it works
============

SamplerBox uses MIDI messages from a connected MIDI keyboard or device to trigger digital audio samples (wave files) which are then converted to
an analogue audio signal. The software has been designed to run on `Raspberry Pi <https://www.raspberrypi.org/>`_ single-board computers. A single-board computer is a tiny computer
that contains a CPU processor, GPU, ROM, RAM, Ethernet, USB and HDMI ports. They can be programmed to do almost anything: run an operating system,
operate a security system, navigate aircraft, take over the world. In the case of SamplerBox its sole purpose is to play music!

Once SamplerBox is running, it will find sample-set directories on a connected USB drive and add them to a setlist. SamplerBox will then attempt to load sample files based on a file naming convention
or filenames and rules defined in a definition.txt file.


Documentation
-------------
This is a rework of the  original samplerbox with the best of the best of the best and... 
+ user-Interface can be connected over serial cable (5V, GND, sda, scl, INT) - don't forget the level-shifter
  - the 16x2 LCD can be connected via i2c (PCF8574)
  - the buttons ban be connected via i2c + INT-pin (PCF8574) 

- samples are located on a third partition mounted at /samples or on USB-flash-drive mounted at /media

- configuration is done in boot-partition

- it is possible to create multi-sample-sets with different samples/voices for each channel
  (see example definitions.txt)

+ midi over OSC
+ translated to python3

- testet and running on pi zero-w(1.1) with i2s-soundcard and usb-midi
  
More in-depth documentation can be found `here <http://samplerbox.readthedocs.io/>`_.

Contributors
------------

+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Joseph Ernest** |twitter: `@JosephErnest <http:/twitter.com/JosephErnest>`_ mail: `contact@samplerbox.org <mailto:contact@samplerbox.org>`_              |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Alex MacRae**   |web: `GitHub <https://github.com/alexmacrae/SamplerBox>`_ mail: `alex@samplerbox.org <mailto:alex@samplerbox.org>`_                     |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Pavel Titov**   |                                                                                                                                        |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Hans Hommersom**|web: http://homspace.xs4all.nl/homspace/samplerbox/index.html                                                                           |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Erik**          |web: http://www.nickyspride.nl/sb2/                                                                                                     |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+
|**Sueppchen**     |                                                                                                                                        |
+------------------+----------------------------------------------------------------------------------------------------------------------------------------+


License
-------

`Creative Commons BY-SA 3.0 <http://creativecommons.org/licenses/by-sa/3.0>`_

