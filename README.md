README.md
==========

([Hotshot instructions](https://github.com/jtzl/offlabelos#just-the-facts))

Off-Label OS is an adventure in technology, a different kind of software experience--part puzzle, part poetry.  It's a little hard to explain concisely at the moment, but think of it as an open-ended computer game in which the computer is the game.  The best way to get a sense of it, of course, is to do.  To get started, you need to install some software first.

Requirements
-----------

Before downloading or installing anything, be sure to have/do the following:

* Modern computer (Mac / Win / Linux -- my 1.6GHz i5 laptop suffices)
* 4GB+ RAM
* 6GB+ free disk space (at the very least)
* Agree to [EULA](https://github.com/jtzl/OffLabelOS/blob/master/LICENSE.txt)

Dependencies
-----------

Off-Label OS runs as a virtualized operating system in your computer (*in* the computer??).  To make it run, you need:

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](http://downloads.vagrantup.com)
* [OffLabelOS.zip](http://offlabelos.com/OffLabelOS.zip.torrent)

If you're totally confused, check out the [video at OffLabelOS.com](http://offlabelos.com/2013/11/01/getting-started-with-olos-part-1-fulfilling-dependencies/).  If you're a little confused but tech savvy-ish, install VirtualBox and then Vagrant.  Personally, I've had problems with the newest Virtualbox but have successfully used Off-Label OS with VirtualBox v 4.2.18 with Vagrant 1.3.3 and VirtualBox 4.2.4 with Vagrant 1.2.2.  If you use different versions, please share the details!

Installation
-----------

After installing VirtualBox and Vagrant, download and unzip the [OffLabelOS.zip](http://offlabelos.com/OffLabelOS.zip.torrent) file, which is available freely and legally via torrent.

Before unzipping OffLabelOS.zip, it's a good idea to verify that your .zip file is the same one that I uploaded, which you can by verifying the pgp signature, probably by using gpg.  [Download the key here](http://offlabelos.com/OffLabelOS.sig).  Learn how to [verify key signatures here](http://offlabelos.com/2013/11/03/pgp-keys-with-gpg/).

After unzipping OffLabelOS.zip, you need to use the command-line interface to start vagrant, but this is super-simple so don't give up yet; you've come so far...  When you launch your command-line terminal, use the `cd` command to get to the directory where the unzipped OffLabelOS directory lives (probably ~/Downloads/OffLabelOS).  Once there, enter `vagrant box add OffLabelOS_v001 OffLabelOS_v001.box` at the prompt and press return.  This loads the OLOS vagrant ".box" file into VirtualBox and makes it accessible via Vagrant.

Finally, type `vagrant up` in this same directory and press return.  At this point, a new window from VirtualBox should pop open and start to load Off-Label OS and eventually present you with a login prompt.

If you get this far, email me for the login / pass:  offlabelos@gmail.com  (v1 luddite metrics-gathering strategy)


Just the facts
===============
Gonna get right to it, eh?  Don't forget, [you accept responsibility for yourself and your systems](https://github.com/jtzl/OffLabelOS/blob/master/LICENSE.txt)

* Download & Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) (4.2.x seems to be good)
* Download & Install [Vagrant](http://downloads.vagrantup.com) (1.2.x or 1.3.x both seem to work)
* Download [OffLabelOS.zip](http://offlabelos.com/OffLabelOS.zip.torrent) (2GB via torrent)
* Download [OffLabelOS.sig](http://offlabelos.com/OffLabelOS.sig)
(See [valid signatures here](https://github.com/jtzl/OffLabelOS/blob/master/CHANGELOG.md))

Command-line time:

* `gpg --recv-keys 8F1D6125` (2011 83C3 1C8D B187 D019  2065 0040 1F2F 8F1D 6125)
* `gpg --verify OffLabelOS.sig OffLabelOS.zip`
* `unzip OffLabelOS.zip`
* `cd OffLabelOS`
* `vagrant box add OffLabelOS_v001 OffLabelOS_v001.box`
* `vagrant up`
