dotnet.py
=========

python script to detect .net framework installed on your PC.

Author: Yong Zhao (zonplm At gmail dot com)
Date:   2012-05-22
Rev:    0.1    
  

-Prerequisite

  You need to have a working python installed on your windows desktop.
  check http://www.python.org/download/
  
-Usage

    donet.py [--machine|-m=<computer_name>] [--check|-c=all|1.0|1.1|2.0|3.0|3.5|4]
    if invoked with a 32 bit python, 32 bit versions of .net framework will be returned;
    if invoked with a 64 bit python, 64 bit versions of .net framework will be returned.

-Sample Run:

    C:\IronPythonPlay>'C:\Program Files (x86)\IronPython 2.7.1\ipy64.exe' dotnet.py
    
    2.0.50727.5420     SP2  -     None
    3.0.30729.5420     SP2  -     None
    3.5.30729.5420     SP1  64bit C:\Windows\Microsoft.NET\Framework64\v3.5\ 
    4.0.30319:Client   GA   64bit C:\Windows\Microsoft.NET\Framework64\v4.0.30319\ 
    4.0.30319:Full     GA   64bit c:\Windows\Microsoft.NET\Framework64\v4.0.30319\ 
    
    C:\IronPythonPlay>"C:\Program Files (x86)\IronPython 2.7.1\ipy.exe" dotnet.py 
    
    2.0.50727.5420     SP2  -     None
    3.0.30729.5420     SP2  -     None
    3.5.30729.5420     SP1  32bit C:\Windows\Microsoft.NET\Framework\v3.5\ 
    4.0.30319:Client   GA   32bit C:\Windows\Microsoft.NET\Framework\v4.0.30319\  
    4.0.30319:Full     GA   32bit c:\Windows\Microsoft.NET\Framework\v4.0.30319\ 

-Misc.

	For information on .net installation registry keys, see:
	http://support.microsoft.com/kb/318785
	http://msdn.microsoft.com/en-us/library/hh925568(v=vs.110).aspx
	http://msdn.microsoft.com/en-us/library/hh925567(v=vs.110).aspx