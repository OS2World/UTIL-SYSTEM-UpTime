  Tue Jun 11 11:54:38 GMT 1996
  
  uptime.exe by Cheng-Yang Tan, cytan@tristan.tn.cornell.edu
  
  Description:
  	a UNIX like uptime application.
  
  To make:
  	gcc -Zomf -o uptime.exe uptime.c uptime.def
  	
  dependencies:
  	dqps.h	
  	
  The source below demonstrates usage of:
  	(1) the undocumented API DosQProcStatus	
  	(2) the thunking macros of emx-gcc version 2.7.2
  	(3) the documented API DosQuerySysInfo
  	
  Acknowledgements:
  	Tomas �gren, stric@arbornet.org who wrote cstart from which I copied
  			     the code for getting the "uptime".
  			     
    Kai Uwe Rommel, for his excellent documentation on DosQProcStatus
    	available at ftp.leo.org in directory /pub/comp/os/os2/doc as proc.zip
    	
    Eberhard Mattes, for his documentation on the thunking macros of emx-gcc
    	available as emxdev.inf in the emx09b distribution.
    	
    IBM for making OS/2.    	
    	
  Copyright:
  	I release this code into the public domain *except* where the copyrights
  	are held by the individual authors above.  I hold no responsibility for the
  	usage of this code.

*** UPDATED by Brian Smith 3-16-98 ***
On my system the time was incorrectly shown. So I edited it to use the DosGetDateTime
API instead.  If there are any problems email me at dbsoft@technologist.com
