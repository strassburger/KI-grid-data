# KI-grid-data
King Island grid data:  
How to get data of King Island and put it into files.

the source:
http://www.kingislandrenewableenergy.com.au/kiapp-dashboard/dashboard.html

the source was  found this way:
start http://www.kingislandrenewableenergy.com.au/

copy this to your local machine

Here search or ask a good friend like i did. Thank you Thorsten.

The idea now is:

open the source page, mark all text with ctrl+a, copy it with ctrl+c and paste it with crtl+v into a file.
Now you only need for any copy + paste a timestamp also.

The ki-scriptxx just do it for you  if you have a ubuntu linux machine
Extra Tools / look for other tools if you use other OS like windows:
The machine also need "xdotool" installed for sending auto keystrokes from script
The machine needs "xsel" installed for putting data from clipbord to datafile

#untill ki-script16: Only the machine can not be used for working. 
# ki-script 17 solved the problem but a little trap: do not use Ctrl+C, should be fine with Ctrl+Insert
The data separator is now ";".

If the data do not change in the  dashboard 
Verify with http://www.kingislandrenewableenergy.com.au/ 
Wait 2 Minutes
1.if there are also no change the data is not send .
2.if there are changes start the script new


But it could be optimized and adapted to your OS.
Have fun
Version changes:

ki-script15:
new data output format

ki-script16:
correction of data file name change if date changes

ki-script17:
script working without gedit.
Data every 2 second
machine should not be blocked, means can be used for other job
only firefox window "king Island showcase" should not be closed or be opend second time. 

Still open points:
copy and paste do not work in other appl1cations.....
check for missing data and delete the incomplete data line
Output in reduced and averaged 1min / 5min / 10 min form to have reduced data volume

 
 





 
