# zerodownsw-update
Update files for ZeroDown Software
***********************************************
*    ZeroDown Software Update Utility
*
***********************************************

Update 2019-06-26
===================
Updated Downloads link to HTTPS.

Update 2019-05-13
===================
Updated self-signed certificate that expired and prevented switch and node from loading properly


Update 2019-01-31
===================

Fixed local volume mapping for nodes and switches.



Update: 2018-10-04
===================

This update package contains 3 files

update.sh	update script to update from version 8.05 and prior

zds-usr.tar	update pacakge for ZeroDown Software

zds-etc.tar	update package for ZeroDown Software system files

Update: 2018-12-30
===================

Fixes Internet Explorer browser issue with reactive interface


***********************************************
*      Instructions
***********************************************

1.)	Download the update utility to the ZeroDown Software instance.  Any SSL Certificates and Configurations will
    need to be reinstalled/configured.  Backup the SSL Certificate prior to updating ZeroDown Software.  
    Login authentication will revert to default admin credentials.

zdsupdate.tar 

or from the ZeroDown Software instance:

wget https://downloads.zerodownsoftware.com/zdsupdate/zdsupdate.tar


2.)	Unpack the compressed update utility scripts and files

tar xvf zdsupdate.tar


3.)	Run the update script from an elevated user

sudo ./update.sh


4.)	Restart the services with the following commands:

sudo zds-ui restart

sudo zerodown restart
