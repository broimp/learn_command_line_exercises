#### Chapter_19 man

> What option to ls tells it to output file size in human readable form?

```
It must be the -h option. Though B's and K's would only be human-sensible
to a tiny subset of humanity.

Brookss-MBP:learn_command_line_exercises $ ls -ahl
total 40
drwxr-xr-x  30 bi  staff   1.0K Feb 26 18:37 .
drwxr-xr-x  10 bi  staff   340B Feb 24 18:58 ..
-rw-r--r--@  1 bi  staff   8.0K Feb 15 11:08 .DS_Store
drwxr-xr-x  15 bi  staff   510B Feb 29 09:36 .git
drwxr-xr-x   9 bi  staff   306B Feb 29 09:36 .idea
drwxr-xr-x   4 bi  staff   136B Feb 28 12:49 Chapter_1
drwxr-xr-x   4 bi  staff   136B Feb 22 21:29 Chapter_10
drwxr-xr-x   5 bi  staff   170B Feb 25 13:11 Chapter_11
drwxr-xr-x   5 bi  staff   170B Feb 28 13:23 Chapter_12
drwxr-xr-x   4 bi  staff   136B Feb 26 11:10 Chapter_13
drwxr-xr-x   4 bi  staff   136B Feb 26 12:07 Chapter_14
drwxr-xr-x   4 bi  staff   136B Feb 26 14:31 Chapter_15
drwxr-xr-x   4 bi  staff   136B Feb 28 09:52 Chapter_16
drwxr-xr-x   4 bi  staff   136B Feb 26 19:08 Chapter_17
drwxr-xr-x   4 bi  staff   136B Feb 29 09:35 Chapter_18
drwxr-xr-x   4 bi  staff   136B Feb 28 20:25 Chapter_19
drwxr-xr-x   4 bi  staff   136B Feb 14 14:52 Chapter_2
drwxr-xr-x   4 bi  staff   136B Feb 28 20:46 Chapter_20
drwxr-xr-x   4 bi  staff   136B Feb 28 21:17 Chapter_21
drwxr-xr-x   4 bi  staff   136B Feb 28 21:55 Chapter_22
drwxr-xr-x   4 bi  staff   136B Feb 28 22:30 Chapter_23
drwxr-xr-x   3 bi  staff   102B Feb 12 11:58 Chapter_3
drwxr-xr-x   5 bi  staff   170B Feb 13 19:10 Chapter_4
drwxr-xr-x   5 bi  staff   170B Feb 16 15:42 Chapter_5
drwxr-xr-x   5 bi  staff   170B Feb 16 16:57 Chapter_6
drwxr-xr-x   4 bi  staff   136B Feb 16 18:32 Chapter_7
drwxr-xr-x   7 bi  staff   238B Feb 16 18:34 Chapter_8
drwxr-xr-x   4 bi  staff   136B Feb 24 10:40 Chapter_9
-rw-r--r--   1 bi  staff    65B Feb 11 17:07 README.md
-rw-r--r--   1 bi  staff   3.0K Feb 26 18:38 all_videos.txt

```

> Is there a case insensitive option to grep?

```
Yes, that's the -i option.
```

> What does the -r and -f options to rm do exactly?

```
The -r option applies the rm command recursively to subdirectories from the starting dir.
The -f option executes removals without prompting.
```

> What does the ifconfig command do?

```
DESCRIPTION
     The ifconfig utility is used to assign an address to a network interface
     and/or configure network interface parameters.

     The following options are available:

     address
             For the DARPA-Internet family, the address is either a host name
             present in the host name data base, hosts(5), or a DARPA Internet
             address expressed in the Internet standard ``dot notation''.
```

> Man files from flashcard topics

```
Copying text out from these files into mines or pbcopy isn't working too well - lots
of doubled characters.

I made separate txt files for each of the subject commands and had planned to add
those to the commit for this chapter, but they have doubled chars too.

Turns out, this is a familiar problem:
    
    http://stackoverflow.com/questions/26634497/redirecting-man-page-output-to-file-results-in-double-letters-in-words
    
    The 'man' program was originally designed to print its output on teletypes, and uses over-printing
    to produce bold character and underlining effects. What you're actually seeing is the effect of the 
    file containing strings of the form X^HX, where the ^H is a backspace character. You also have 
    strings like _^HX, for underlining (hence the _f_i_l_e).
    
    These can be stripped easily using a text editor like vi, which will display the backspaces.
    
    :%s/_^H//g
    will remove the underlines, and
    
    :%s/.^H.//g
    the boldings (the ^H in the above is ctrl-H. You will have to use ctrl-V ctrl-H to enter these into vi.


In short, a research project for another day...
```
