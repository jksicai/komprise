# komprise
Useful Komprise Tools for SEs and Komprise Customers

Source of this script is Eric Platt/Komprise Eng

This script is used to generate mutiple files for a lab or testing environment.  


The syntax is below.

sudo python ~/tmp/dofiles.py gen /home/kompuser/tmp/src/dofiles/Iter1 1000 10240000 10240
 
PATH - absolute path on the machine where share is mounted to populate data
Whichever of NUMFILES or SIZEFILES is reached first stops the script.
The average filesize is 1MB.
If FILESIZE is specified, all files are created dense at that fixed size.

Here is an example to create 1000 files and each of 10KB size.

sudo python ~/tmp/dofiles.py gen /home/kompuser/tmp/src/dofiles/Iter1 1000 10240000 10240
