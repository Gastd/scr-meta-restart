scr-meta-restart
================

Patch for [TORCS](http://torcs.sourceforge.net/) and SCR to restart the race by setting the ```meta``` parameter.

Installation
------------

This is a patch, it modifies the software's source files, so _you will have to reinstall TORCS for changes to have effect_. 

As per the "_Simulated Car Racing Championship Competition Software Manual_" ([v2 - April 2013](http://arxiv.org/pdf/1304.1672v2)), download [TORCS](http://torcs.sourceforge.net/index.php?name=Sections&op=viewarticle&artid=3) and the [SCR patch](http://sourceforge.net/projects/cig/files/SCR%20Championship/Server%20Linux/) files, extract them and apply the patch. *Do not configure/install TORCS yet*.

After applying the SCR patch, extract the ```scr-meta-restart``` patch into your TORCS folder and apply it:

    cd scr-meta-restart
    sh do_patch.sh

Then finish the TORCS installation in the usual manner (from the TORCS folder):

    ./configure
    make
    sudo make install
    sudo make datainstall

Use
---

The patch simply makes the SCR server tell the TORCS race engine to restart the race, as specified in the [Official TORCS FAQ](http://torcs.sourceforge.net/index.php?name=Sections&op=viewarticle&artid=30#c6_8). 

In practice, this means that *INSERT MEANING HERE*.

Here is a simple example: *INSERT EXAMPLE HERE*

Support
-------

The provided software is available *as is*, without warranty or support of any kind. We are, however, open to productive collaborations to improve the software. If you're using it, please link to this page.

This patch was tested on: (let us know your systems specifications if it works for you - sorry if it doesn't)

* Ubuntu 14.04 (64 bits), TORCS v1.3.6
