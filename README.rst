
ElectrumX Banner Updater
------------------------

This script can be used to update the ElectrumX banner file to contain information about memory pool and fees.

ElectrumX server: 
    https://github.com/Electrum-RVN-SIG/electrumx-ravencoin
    
Bitcoin Core daemon:
    https://github.com/RavenProject/Ravencoin


Getting Started
---------------

The first time you run this script your original banner file will be copied to ``${BANNER}.template``.

On each subsequent run ``${BANNER}.template`` will be used as the top portion of the new banner.

If you wish to change your banner you should edit ``${BANNER}.template``.


Edit update-electrumx-banner:
*****************************

- Adjust the ``RAVENCOIN_DATADIR`` environment to specify where to find your ravencoin data directory.

- Adjust the ``RAVENCOIN_CLI`` environment to specify where to find raven-cli.

- Adjust the ``BANNER`` environment to specify the your electrumx banner file.


Scheduled Update:
*****************

Run ``crontab -e`` and add a cron job to update the banner every 2 minutes.

::

    */2 * * * *  /path/to/update-electrumx-banner


Versions
--------

This script is working with the following software versions::

 Operating System:   Ubuntu 20.10
 ElectrumX Ravencoin:1.8.0
 Ravencoin Core:     4.3.2.1


=======================================================

**Samuel Smith**  shsmith@socal.rr.com   https://github.com/shsmith
