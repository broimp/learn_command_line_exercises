Make 20 more directories and remove them all.

  Brookss-MBP:Chapter_7 $ cd tmp
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ mkdir -p 1/2/3/4/5/6/7/8/9/10/11/12/13/14/15/16/17/18/19/20
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ tree
  .
  ├── 1
  │   └── 2
  │       └── 3
  │           └── 4
  │               └── 5
  │                   └── 6
  │                       └── 7
  │                           └── 8
  │                               └── 9
  │                                   └── 10
  │                                       └── 11
  │                                           └── 12
  │                                               └── 13
  │                                                   └── 14
  │                                                       └── 15
  │                                                           └── 16
  │                                                               └── 17
  │                                                                   └── 18
  │                                                                       └── 19
  │                                                                           └── 20
  └── stuff
      └── things
          └── frank
              └── joe
                  └── alex
                      └── john
  
  26 directories, 0 files
    
  Brookss-MBP:tmp $ rm -r 1
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ pwd
  /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_7/tmp
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ tree
  .
  └── stuff
      └── things
          └── frank
              └── joe
                  └── alex
                      └── john
  
  6 directories, 0 files
  
Make a single path of dirs that is 10 deep and remove them one at a time.

  Brookss-MBP:tmp $ mkdir -p 1/2/3/4/5/6/7/8/9/10
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ cd ./1/2/3/4/5/6/7/8/9/10
  
  (master) Brooks Imperial
  Brookss-MBP:10 $ pwd
  /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_7/tmp/1/2/3/4/5/6/7/8/9/10
  
  (master) Brooks Imperial
  Brookss-MBP:10 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:9 $ rmdir 10
  
  (master) Brooks Imperial
  Brookss-MBP:9 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:8 $ rmdir 9
  
  (master) Brooks Imperial
  Brookss-MBP:8 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:7 $ rmdir 8
  
  (master) Brooks Imperial
  Brookss-MBP:7 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:6 $ rmdir 7
  
  (master) Brooks Imperial
  Brookss-MBP:6 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:5 $ rmdir 6
  
  (master) Brooks Imperial
  Brookss-MBP:5 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:4 $ rmdir 5
  
  (master) Brooks Imperial
  Brookss-MBP:4 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:3 $ rmdir 4
  
  (master) Brooks Imperial
  Brookss-MBP:3 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:2 $ rmdir 3
  
  (master) Brooks Imperial
  Brookss-MBP:2 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:1 $ rmdir 2
  
  (master) Brooks Imperial
  Brookss-MBP:1 $ cd ..
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ rmdir 1
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $ ls
  stuff
  
  (master) Brooks Imperial
  Brookss-MBP:tmp $
  
Can you remove the tmp direcory?

  Not with the rmdir command.
  
  Brookss-MBP:Chapter_7 $ rmdir tmp
  rmdir: tmp: Directory not empty
  
Remove the tmp directory.

  Brookss-MBP:Chapter_7 $ rm -r tmp
  
  (master) Brooks Imperial
  Brookss-MBP:Chapter_7 $ pwd
  /Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_7
  
  (master) Brooks Imperial
  Brookss-MBP:Chapter_7 $ tree
  .
  └── Readme.md
  
  0 directories, 1 file
  
  If any of the subdirectories contained files, and they were to be also removed,
  use the "rm -rf" command.

  
  
  
  
  
  
