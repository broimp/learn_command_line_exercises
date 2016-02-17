####Explain what the pushd and popd commands do.

  Pushd, followed by a directory path argument like dot for the current directory,
  makes a copy of the specified directory path in the pushd/pod stack.
  
  The stack is LIFO - last in first out. I just tested it two deep. Keeping a stack
  of directories to access might be useful for some sort of system maintenance. Probably 
  not of much utility in dynamic command line work.

####Explain what directories I used to test pushd/popd.

  I used the following:
```  
  Brookss-MBP:Chapter_8 $ tree
  .
  ├── Readme.md
  ├── i
  │   └── like
  │       └── icecream
  ├── temp
  │   └── stuff
  │       └── things
  │           └── frank
  │               └── joe
  │                   └── alex
  │                       └── john
  └── with
      └── my
          └── cake
  
  13 directories, 1 file
```
