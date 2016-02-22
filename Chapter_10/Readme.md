> Can you copy the foo.txt file to slash temp? (Create foo.txt first...)

```
Brookss-MBP:Chapter_10 $ ls
Readme.md

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ mkdir temp

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ echo 'foo' > foo.txt

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ cp ./foo.txt ./temp/.

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ tree
.
├── Readme.md
├── foo.txt
└── temp
    └── foo.txt

1 directory, 3 files
```

> Can you copy .bash_profile in your home directory to the current directory?

```
Brookss-MBP:Chapter_10 $ cp $HOME/.bash_profile .

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ ls -la
total 24
drwxr-xr-x   7 bi  staff  238 Feb 22 12:59 .
drwxr-xr-x  16 bi  staff  544 Feb 22 12:50 ..
-rw-r--r--   1 bi  staff  852 Feb 22 12:59 .bash_profile
```

> Explain robocopy

Robocopy is a windows command for keeping multiple copies of directory structures and the files they contain.

> Use the cp -r command to copy more directories with files in them.

This command copies directories and/or their contents.

```
 -R    If source_file designates a directory, cp copies the directory and
           the entire subtree connected at that point.  If the source_file
           ends in a /, the contents of the directory are copied rather than
           the directory itself.  This option also causes symbolic links to be
           copied, rather than indirected through, and for cp to create spe-
           cial files rather than copying them as normal files.  Created
           directories have the same mode as the corresponding source direc-
           tory, unmodified by the process' umask.

           In -R mode, cp will continue copying even if errors are detected.
```

Copy a file to your home directory or desktop.
```
Brookss-MBP:Chapter_10 $ echo 'junk' > junk.file

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ cp ./junk.file $HOME/.

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ ls $HOME | grep junk
junk.file

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ rm $HOME/junk.file

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $ ls $HOME | grep junk

(master) Brooks Imperial
Brookss-MBP:Chapter_10 $
```

> Find these files in your graphical user interface and open them in a text editor.

This involves using Finder to locate the files. 

> Notice how sometimes I put a / (slash) at the end of a directory? That makes sure the file is really a directory, so if the directory doesn't exist I'll get an error.

It's always appropriate to use the most specific item address available to limit unintended consequences.
