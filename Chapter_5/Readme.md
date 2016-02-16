Do More exercises

  cd to the joe directory with one command
    Find the "Joe" dir in finder, copy "Joe" to put the "Joe" path into copy buffer
    
    Brookss-MBP:Chapter_5 $ cd /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_4/temp/stuff/things/frank/joe
    
  cd back to temp with one command, but not further above that

    Brookss-MBP:joe $ cd ../../../..
    
    (master) Brooks Imperial
    Brookss-MBP:temp $ pwd
    Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_4/temp
    
  cd to home directory with one command
    cd or cd ~
    Brookss-MBP:~ $ pwd
    /Users/bi
    
  cd to your Documents directory then find it with your GUI file browser
    Brookss-MBP:~ $ ls
    Applications    Documents       Movies          Pictures
    BitTorrent Sync Downloads       Music           Public
    Desktop         Library         OReilly Ed      workspace
    
    
    Brookss-MBP:~ $ cd Documents
    
    
    Brookss-MBP:Documents $ pwd
    /Users/bi/Documents
    
    Finding Documents with the file browwer is interesting. It appears that the first
    Documents directory displayed is the directory, followed by a number of library
    pointers that refer back to the Documents directory. The real Documents directory
    has a feint outline of a folder inside the blue folder, whereas the pointer items
    don't contain that outline. This is a little subtle.
    
  cd to your Downloads directory, then find it with your file browser.
  
    Brookss-MBP:~ $ pwd
    /Users/bi
    
    Brookss-MBP:~ $ ls
    Applications    Documents       Movies          Pictures
    BitTorrent Sync Downloads       Music           Public
    Desktop         Library         OReilly Ed      workspace
    
    Brookss-MBP:~ $ cd Downloads  
    Brookss-MBP:Downloads $

    In Finder, downloads had a main directory item with a path to it, and only 
    one pointer item to another application tracking it.
    
  Find another directory with your file browser, then cd to it.
  
    Typing in "learn" in the Finder search bar, learn_command_line_exercises directory comes up.
    
    Brookss-MBP:homework $ cd /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
    
  Remember when you put quotes around a directory with spaces in it? You can do that with any command. For example, if you have a directory I Have Fun, then you can do: cd "I Have Fun"
  
    Brookss-MBP:learn_command_line_exercises $ cd /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_4/temp/I\ Have\ Fun
    
    (master) Brooks Imperial
    Brookss-MBP:I Have Fun $
    
    Brookss-MBP:I Have Fun $ cd ..
    
    (master) Brooks Imperial
    Brookss-MBP:temp $ cd "I Have Fun"
    
    (master) Brooks Imperial
    Brookss-MBP:I Have Fun $
    
    I note that the path Finder gave me for "I Have Fun" did not contain quotes. It
    had reverse slashes in it. The backslash at terminal level apparently cause
    the embedded spaces to be treated literally as part of the surrounding string,
    according to one writer.
    
    I did not get this to work by typing in I \Have \Fun, so this is still an 
    open question. Quotations surrounding the string work fine.
    
  ------------
  
  Can you cd into the temp directory?
    Yes, directory path gleaned from Finder.
    Brookss-MBP:temp $ cd /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_5/temp
    
  Why don't we go into the temp directory?
    Brookss-MBP:temp $ pwd
    /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_5/temp
    
    Well, we do go into the temp directory, so I can't validate this question.
    
  Can you go to the /tmp directory?
  
    Yes. The /tmp directory at root does not persist between login sessions.
    
    Brookss-MBP:Chapter_5 $ cd /tmp
    
    Brookss-MBP:tmp $ pwd
    /tmp
      
    Brookss-MBP:tmp $ ls -la
    total 576
    drwxrwxrwt  10 root  wheel     340 Feb 16 13:48 .
    drwxr-xr-x@  6 root  wheel     204 Oct 17 17:38 ..
    -rw-rw-rw-@  1 bi    wheel       0 Feb 15 17:52 .keystone_install_lock
    drwx------   3 bi    wheel     102 Feb 16 12:04 KSOutOfProcessFetcher.501.sAglCyxY5lzPoNgfmEvv-ZqGl-w=
    drwx------   3 bi    wheel     102 Feb 15 17:48 com.apple.launchd.MX5k7JSgAC
    drwx------   3 bi    wheel     102 Feb 15 17:48 com.apple.launchd.mUoShFnNSS
    -rw-r--r--@  1 bi    wheel       0 Feb 15 17:48 ct.shutdown
    drwxr-xr-x   2 bi    wheel      68 Feb 16 09:58 log
    -rw-r--r--   1 root  wheel   71296 Feb 15 18:26 wifi-Gkqia8.log
    -rw-r--r--   1 root  wheel  219569 Feb 15 17:56 wifi-g5zarG.log
    
  Can you go to the /tmp/log directory?
  
    Yes
    Brookss-MBP:tmp $ mkdir log
    
    Brookss-MBP:tmp $ ls -la | grep log
    drwxr-xr-x   2 bi    wheel      68 Feb 16 15:31 log
    
    Brookss-MBP:tmp $ cd log
    
    Brookss-MBP:log $ pwd
    /tmp/log
   
    
  What does the .. argument to cd do?
  
    That says change the present working directory to the parent directory of 
    the directory you are in. In other words, go up one level in the directory tree.
    
    
    
    
    
