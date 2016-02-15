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
    
  Can you go to the slash temp directory?
  
    There is no /temp directory. That would be a temp directory at the root, and the 
    temp diretories are hanging off Chapter directories.
    
  Can you go to the slash temp slash log directory?
  
    No, you can't go there either. The log directory is not a subdirectory of
    either temp directory. 
    
  What does the .. argument to cd do?
  
    That says change the present working directory to the parent directory of 
    the directory you are in. In other words, go up one level in the directory tree.
    
    
    
    
    
