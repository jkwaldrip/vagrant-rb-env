# A Ruby Development Environment in Vagrant
---

## Installation

The creators of Vagrant have helpfully provided installers for all major operating systems:

  https://docs.vagrantup.com/v2/installation/

To use this Vagrant configuration, you'll need to install VirtualBox to serve as the provider
for virtual machines.  There's a download link available from the Vagrant documentation, as
well as a short note on which VirtualBox versions are compatible with the current release of
Vagrant:

  http://docs.vagrantup.com/v2/virtualbox

With Vagrant installed and VirtualBox as a virtual machine provider, 
clone this repository to your preferred Vagrant directory, then
in a shell session, navigate to this directory and run:

    $ vagrant up

This will download the official Ubuntu 32-bit 14.04 (Trusty Tahr) VirtualBox machine,
then bring it online and install both RVM and Ruby.  Please note that downloading the
VirtualBox machine and installing Ruby will run for some time without output, so please
allow at least 15-30 minutes for these steps to complete.

## SSH Access

On a non-Windows environment, you can access the Vagrant virtual machine by running
the following command from this directory:

    $ vagrant ssh

If you're running Vagrant on a Windows environment, you'll probably want to use [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/)
to connect to your running Vagrant machine.  PuTTY will need to be able to access Vagrant's
SSH key in order to connect.  Instructions for getting PuTTY to connect to Vagrant with the
shared SSH key can be found here:

https://github.com/Varying-Vagrant-Vagrants/VVV/wiki/Connect-to-Your-Vagrant-Virtual-Machine-with-PuTTY

## Shut It Down!

When you're done with your Vagrant session, you can exit SSH at any time with the exit command.
To bring your virtual machine to a halt, run the following command from this directory:

    $ vagrant halt

