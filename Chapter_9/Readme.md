On the Do More, make a directory, put a file in it, go back a level, try to remove the directory

  The remdir temp to remove the temp directory fails with a "directory not empty" error.
  
  We can empty the directory manually and then rmdir it.
  We can rm -iR the directory and get a prompt to delete each item in the directory.
  
  i.e.
  Brookss-MBP:Chapter_9 $ rm -iR temp
  examine files in directory temp? y
  remove temp/a_file? y
  remove temp? y
  
  (which is kind of cool, like having a little chat with your computer)
  
  Or we can rm -rf the directory and force delete the directory and all of its
  contents, regardless of what it contains, without inspecting anything.

Can you touch blah.txt?
Can you touch foo.txt?

  Yes
  
  Brookss-MBP:temp $ touch blah.txt
  
  (master) Brooks Imperial
  Brookss-MBP:temp $ touch foo.txt
  
  (master) Brooks Imperial
  Brookss-MBP:temp $ ls -l
  total 0
  -rw-r--r--  1 bi  staff  0 Feb 15 15:02 blah.txt
  -rw-r--r--  1 bi  staff  0 Feb 15 15:02 foo.txt
  
What happens when you touch an existing item?

  Let's find out.
  
  Brookss-MBP:temp $ ls -l
  total 0
  -rw-r--r--  1 bi  staff  0 Feb 15 15:04 blah.txt
  -rw-r--r--  1 bi  staff  0 Feb 15 15:02 foo.txt
  
  (master) Brooks Imperial
  Brookss-MBP:temp $ touch blah.txt
  
  (master) Brooks Imperial
  Brookss-MBP:temp $ ls -l
  total 0
  -rw-r--r--  1 bi  staff  0 Feb 15 15:05 blah.txt
  -rw-r--r--  1 bi  staff  0 Feb 15 15:02 foo.txt
  
  Touching a file changes the mod date/time stamp.
  
  
  
