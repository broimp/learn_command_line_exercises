#### Chapter_19 man

> What option to ls tells it to output file size in human readable form?

```
Three options deal with ls size, but they don't say anything about being human readable.
 Can't validate the question.

Brookss-MBP:learning_by_doing $ man ls | grep size
     -@      Display extended attribute keys and sizes in long (-l) output.
             number of digits to three or less using base 2 for sizes.
     -k      If the -s option is specified, print the file size allocation in
             file sizes is output on a line before the long listing.
             bined with sort by size
     -S      Sort files by size
             total sum for all the file sizes is output on a line before the
             size of 512 bytes.
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
