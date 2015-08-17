# Undo RM - Hacking the filesystem "UNRM"
## Speaker [Jessica Yu][JessicaYuEmail]
### Slides Available [Here][Slides]

The purpose of this is to be able to undo an rm up to a certain amount of time away  
When a user runs rm, it preforms a "ext4_unlink_at" call in the kernel  


Research Terms:  
* radix
* strace
* inode



[Slides]:
[UNRMSorce]:      https://github.com/flaming-toast/unrm
[JessicaYuEmail]: jyu@eisen.io
