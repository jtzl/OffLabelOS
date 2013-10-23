OffLabelOS
==========

Off-Label OS is a different kind of software experience:  part puzzle, part
poetry.  To get started, you need VirtualBox and Vagrant; if you haven't used
either before, install them in that order.  Personally, I had problems with the
newest Virtualbox, but version 4.2.18 with Vagrant version 1.3.3 worked for me,
as well as VirtualBox 4.2.4 with Vagrant version 1.2.2.  If you use different
versions, please post your results to the comments.

After you have downloaded and installed VirtualBox and Vagrant, you should first
download and unzip the olos.zip file, which is available freely and legally via
torrent.

Once you have unzipped olos.zip, you need to get into the command line interface
to start vagrant.  If you are on Mac or Linux, start your terminal and use the
`cd` command to get to the directory where the unzipped olos directory lives,
probably in ~/Downloads/olos --once you're there, enter `vagrant box add
OffLabelOS_v001 OffLabelOS_v001.box` at the prompt, which will load the contents
of the vagrant.box file into VirtualBox and make it accessible to you in
Vagrant.  When that action has completed, type `vagrant up` in that same
directory and press return.

At this point, a new window from VirtualBox should pop open and start to load
Off-Label OS and eventually present you with a login prompt.
