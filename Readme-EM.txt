
Good idea is to realize it on a VirtualMachine (VM)
In Ubuntu just install VirtualBox
Even in Windows you can install VirtualBox.
https://www.virtualbox.org/

So your working machine still will be fine 
How to get data of King Island and put it into files.
change to adapt to electricitymap.org -EM-
split in two scripts
a  ini file: start firefox and the link to King island data
one call file to be called from ... open till now ....

Ini-script: 
ki-script-EM-INI-01

call script:
ki-script-EM-call-01

output file: EM-ki-JJJJ-MM-DD-xx.txt


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

since 2018-01-20:
check for missing data and delete the incomplete data line
Solved workaround: fast + dirty:
open dada files with Libre office calc ";" as separetor
mark column AP
CTRL+V -->copy column AP
open Sheet2
search for kW
delete fount rows in sheet1
check end of data in sheet1 complete data set?
If not delete incomplete Row
Save the File: Use Text CSV format



Output in reduced and averaged 1min / 5min / 10 min form to have reduced data volume
Solved by Mike: Roger have the solution -> a spread sheet of Mike

New:
produce graphs of data files.
Needed:
Installed python
pyton + Data file in same actual directory

command line Syntax:
phyton "phyton script" "data file without extencion"
phython plot_ki_all-07.py ki-yyyy-mm-date
Example:
phython plot_ki_all-07.py ki-2018-01-19 


data file:
ki-yyyy-mm-dd.txt
Example:
ki-2018-01-19.txt

Still every graph have to be saved by hand.
Next graph shown if window of last graph is closed by hand
advantage:
Zoom in unlimited in graphs and save later on.

 





 
 





 
