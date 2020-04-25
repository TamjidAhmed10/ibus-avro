# Avro phonetic for Linux in IBus
Avro phonetic implementation for Linux in IBus.

## Installation

1. Open terminal/package manager and install following packages:
 
   For Ubuntu or any linux distro__
    
    	sudo apt-get install git ibus libibus-1.0-dev automake autoconf gjs gir1.2-ibus-1.0
	
	
    __For other linux distributions__
    
    You'll need all related build tools like `automake`, `autoconf` etc...
    and Latest __IBus__ from _git_ compiled with _gobject-introspection_ support enabled.

2. Now give the following commands step-by-step:

		git clone git://github.com/sarim/ibus-avro.git
		cd ibus-avro
		aclocal && autoconf && automake --add-missing
		./configure --prefix=/usr
		sudo make install
		

## then reboot.
## Usage
Now go to System Settings -> Language Support

Look at the Keyboard input method system
Select IBus and close the window.
You may need to restart IBus to make everything work.

Try the following command:

ibus restart


Otherwise, a reboot may be required.

## Contributors
 
__IBus Engine__ by __Sarim Khan__ <sarim2005@gmail.com>

[__Avro JavaScript Phonetic Library__](https://github.com/torifat/jsAvroPhonetic) by [__Rifat Nabi__](https://github.com/torifat)

__Avro Phonetic Dictionary Search Library__ by [__Mehdi Hasan Khan__](https://github.com/omicronlab)

__Final edited__ by __tamjid ahmed__ https://www.facebook.com/tamjid.ahmed1

_Licensed under Mozilla Public License 1.1 ("MPL"), an open source/free software license._
