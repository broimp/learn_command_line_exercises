At terminal:
  Can you make a temp directory?
  Yes
    from /Users/bi/workspace/davinci_coders_t1_2016/homework
    cd learn_command_line_exercises/
    mkdir Chapter_4
    cd Chapter_4
    pwd
    mkdir temp
    
  Make the 20 directories in the Chapter_4 directory
    pwd (to confirm temp directory is present working directory)
    mkdir -p stuff/things/frank/joe/alex/john
    mkdir -p stuff2/things2/frank2/joe2/alex2/john2
    mkdir -p stuff3/things3/frank3/joe3/alex3/john3
    mkdir -p stuff4/things4/frank4/joe4/alex4/john4
    tree (check results)
  
  Brookss-MBP:Chapter_4 $ tree
  .
  └── temp
      ├── stuff
      │   └── things
      │       └── frank
      │           └── joe
      │               └── alex
      │                   └── john
      ├── stuff2
      │   └── things2
      │       └── frank2
      │           └── joe2
      │               └── alex2
      │                   └── john2
      ├── stuff3
      │   └── thing3
      │       └── frank3
      │           └── joe3
      │               └── alex3
      │                   └── john3
      └── stuff4
          └── thing4
              └── frank4
                  └── joe4
                      └── alex4
                          └── john4
  
  25 directories, 0 files
  
  Can you make a log directory in your class directory?
  
    Use the find command to see if a log directory already exists.
  
    Brookss-MBP:davinci_coders_t1_2016 $ find . log
  
    By default this returns a list of all subdirectories traversed from
    this point to search for log.
  
    At the end:
    find: log: No such file or directory
  
    Conclusion, log does not exist in the class directory, 
    so the answer is yes.
  
    mkdir log
  
  Make a directory with space in the name by putting quotes around it.
    temp$ mkdir "I Have Fun"
    
    Brookss-MBP:temp $ ls -l
    total 0
    drwxr-xr-x  2 bi  staff   68 Feb 11 20:23 I Have Fun
    drwxr-xr-x  3 bi  staff  102 Feb 11 19:25 stuff
    drwxr-xr-x  3 bi  staff  102 Feb 11 19:31 stuff2
    drwxr-xr-x  3 bi  staff  102 Feb 11 19:31 stuff3
    drwxr-xr-x  3 bi  staff  102 Feb 11 19:31 stuff4
    
  
