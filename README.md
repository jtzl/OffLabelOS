Off-Label OS
==========

Off-Label OS is an adventure in technology, a new kind of software experience--part puzzle, part poetry.  The best way to learn, of course, is to do.  To get started, you need to install some software first.

Dependencies
-----------

Off-Label OS runs as a virtualized operating system in your computer (*in* the computer??).  To make it run, you need:

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](http://downloads.vagrantup.com)

If you're totally confused, check out the video at [offlabelos.com](http://offlabelos.com/2013/11/01/getting-started-with-olos-part-1-fulfilling-dependencies/).  If you're a little confused but tech savvy-ish, install VirtualBox and then Vagrant.  Personally, I've had problems with the newest Virtualbox but have successfully used Off-Label OS with VirtualBox v 4.2.18 with Vagrant 1.3.3 and VirtualBox 4.2.4 with Vagrant 1.2.2.  If you use different versions, please share the details!

Installation
-----------

After installing VirtualBox and Vagrant, download and unzip the [OffLabelOS.zip](http://offlabelos.com/OffLabelOS.zip.torrent) file, which is available freely and legally via torrent.

Before unzipping OffLabelOS.zip, it's a good idea to verify that your .zip file is the same one that I uploaded, which you can by verifying the pgp signature, probably by using gpg.  [Download the key here](http://offlabelos.com/OffLabelOS.sig).  [Learn how to verify key signatures here](offlabelos.com/2013/11/03/pgp-keys-with-gpg/).

After unzipping OffLabelOS.zip, you need to use the command-line interface to start vagrant, but this is super-simple so don't give up yet; you've come so far...  When you launch your command-line terminal, use the `cd` command to get to the directory where the unzipped OffLabelOS directory lives (probably ~/Downloads/OffLabelOS).  Once there, enter `vagrant box add OffLabelOS_v001 OffLabelOS_v001.box` at the prompt and press return.  This loads the OLOS vagrant ".box" file into VirtualBox and makes it accessible via Vagrant.

Finally, type `vagrant up` in this same directory and press return.  At this point, a new window from VirtualBox should pop open and start to load Off-Label OS and eventually present you with a login prompt.
