# Undo RM - Hacking the filesystem "UNRM"
### Speaker [Jessica Yu][JessicaYuEmail]
### Slides Will Be Available [Here][Slides]

The purpose of this is to be able to undo an rm up to a certain amount of time away  
When a user runs rm, it preforms a "ext4_unlink_at" call in the kernel  
There is a list of stuff that she needs help with, such as:
* Security
  * Non-Root Users can execure this
* Memory Consumption
  * if you delete a massive amount of data, it all lives in ram until the timer expieres
  * I suggest this: have a way to delete WITH OUT option of recovery (-f for no recovery?)
* Hard Coded Timer
  * Need to find a way to change the default timer (on a per rm?) its hard coded to 30seconds right now

Research Terms:
* radix
* strace
* inode

Want to see for yourself? [Github Link][UNRMSource]


[Slides]:
[UNRMSorce]:      https://github.com/flaming-toast/unrm
[JessicaYuEmail]: jyu@eisen.io
