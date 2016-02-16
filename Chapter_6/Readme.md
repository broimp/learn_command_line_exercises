####Describe what ls -lR does.
  List directory contents in long format, and shows all subordinate directories in long
  format too.
  
  Long format displays the user/group/3rd party rights to read (r), write (w), and execute (x) the
  file. The rights are either present, or absent which is indicated by a dash. 
  The first character in the permissions string contains a (d) if the item
  is a directory.

```
  Brookss-MBP:Chapter_6 $ ls -lR
  total 0
  -rw-r--r--  1 bi  staff    0 Feb 15 12:42 Readme.md
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 tmp
  
  ./tmp:
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 stuff
  
  ./tmp/stuff:
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 things
  
  ./tmp/stuff/things:
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 frank
  
  ./tmp/stuff/things/frank:
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 joe
  
  ./tmp/stuff/things/frank/joe:
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 alex
  
  ./tmp/stuff/things/frank/joe/alex:
  total 0
  drwxr-xr-x  2 bi  staff  68 Feb 15 12:13 john
  
  ./tmp/stuff/things/frank/joe/alex/john:
```
####What's in the tmp diretory?
  stuff is in the tmp directory
```  
  Brookss-MBP:tmp $ ls -l
  total 0
  drwxr-xr-x  3 bi  staff  102 Feb 15 12:13 stuff
```  
####Can you show me what files are in that direcory?
```
  I can show you that there are no files in that directory. See previous answer.
  The directory only contains another directory - (d) char is set in the
  permissions string.
```  
####What files are in your home directory?

  Similarly, my home directory only contains other directories. No files.
```  
  Brookss-MBP:tmp $ cd $HOME
  
  Brookss-MBP:~ $ ls -l
  total 0
  drwx------    4 bi  staff   136 Jan 30 12:38 Applications
  drwxr-xr-x    2 bi  staff    68 Feb  5 20:22 BitTorrent Sync
  drwx------+  10 bi  staff   340 Feb  5 23:36 Desktop
  drwx------+  14 bi  staff   476 Feb 15 11:21 Documents
  drwx------+  29 bi  staff   986 Feb 11 18:34 Downloads
  drwx------@  55 bi  staff  1870 Feb  1 19:14 Library
  drwx------+   3 bi  staff   102 Jan 26 19:32 Movies
  drwx------+   4 bi  staff   136 Feb  1 19:14 Music
  drwxrwxrwx  126 bi  staff  4284 Jan 30 05:52 OReilly Ed
  drwx------+   6 bi  staff   204 Feb 12 09:51 Pictures
  drwxr-xr-x+   5 bi  staff   170 Jan 26 19:32 Public
  drwxr-xr-x    6 bi  staff   204 Feb 11 12:24 workspace
```  
####What's in /tmp?

  /tmp is a root level directory that contains files and directories for the
  current session. It's a volatile section that gets rewritten at each login.
```   
  Brookss-MBP:/ $ cd /tmp
      
  Brookss-MBP:tmp $ ls -l
  total 0
  drwx------  3 bi  wheel  102 Feb 15 10:44 KSOutOfProcessFetcher.501.sAglCyxY5lzPoNgfmEvv-ZqGl-w=
  drwx------  3 bi  wheel  102 Feb 15 10:44 com.apple.launchd.DBtVJRgSLt
  drwx------  3 bi  wheel  102 Feb 15 10:44 com.apple.launchd.DLAo1gHLOi
  -rw-r--r--@ 1 bi  wheel    0 Feb 15 10:44 ct.shutdown
  
  The fact that all of these items are dated coincident with my turning on the
  machine this morning indicates that they are session related items.  
  
  Brookss-MBP:tmp $
``` 
  Wiki - https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard 
  - contains following description of /tmp - 
  Temporary files (see also /var/tmp). Often not preserved between system reboots, and may be severely size restricted.
 
  
  


  

  
