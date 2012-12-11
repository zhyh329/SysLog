# SysLog

This is a simple application that records various log types, and compresses them, currently as a tar file.  
The logs are saved under the primary external storage folders named by the date and time.  

Some plans for improvement:
* A popup after the log capture for extra text to be appended to the end of the file/foldername...  or better yet, an extra text file included with the zip that you can enter some notes
* Update the button text to say 'Checking for root' until its enabled
* Switch to Chainfire's SU library
* Clean up the uncompressed log files (Option or pref)
* Option to clear the past log files
* Make sure the SysLog/ dir has a .nomedia file
* Improve root-less operation. (Useless on 4.1+ without root, but I may start lowering the min API level and checking it down to 2.3)
* dmsg without root should work with pre-3.0 kernels, need to check it or always allow it

Done:
* Add last_kmsg support
* Readme/About dialog
* Switch to Zip compression
* Figure out when log files are done being written.

### Note about Root Access:
It may not be possible to get the logs without root access. On 4.2+, this is pretty darn useless without root. Should work, but may have issues with 4.1-
