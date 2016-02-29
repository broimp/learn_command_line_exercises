#### Chapter_23 a few more

> exit

```
This command exits the terminal or shell.
```

> Let's close this terminal and open a new one.
> Can you reload your terminal?

```
Maybe. It looks like SUDO might provide this functionality. I'd have to
research it more.
```

> Can you logout?

```
Yes - logout (same as exit)
```

> xargs

```
XARGS(1)                  BSD General Commands Manual                 XARGS(1)

NAME
     xargs -- construct argument list(s) and execute utility

SYNOPSIS
     xargs [-0opt] [-E eofstr] [-I replstr [-R replacements]] [-J replstr]
           [-L number] [-n number [-x]] [-P maxprocs] [-s size]
           [utility [argument ...]]

DESCRIPTION
     The xargs utility reads space, tab, newline and end-of-file delimited
     strings from the standard input and executes utility with the strings as
     arguments.
```

> sudo

```
SUDO(8)                     System Manager's Manual                    SUDO(8)



NAME
       sudo, sudoedit - execute a command as another user

SYNOPSIS
       sudo -h | -K | -k | -L | -V
       sudo -v [-AknS] [-g group name | #gid] [-p prompt]
            [-u user name | #uid]
       sudo -l[l] [-AknS] [-g group name | #gid] [-p prompt] [-U user name]
            [-u user name | #uid] [command]
       sudo [-AbEHnPS] [-C fd] [-g group name | #gid] [-p prompt]
            [-u user name | #uid] [VAR=value] -i | -s [command]
       sudoedit [-AnS] [-C fd] [-g group name | #gid] [-p prompt]
                [-u user name | #uid] file ...

DESCRIPTION
       sudo allows a permitted user to execute a command as the superuser or
       another user, as specified by the sudoers file.  See the COMMAND
       EXECUTION section below for more details.

```


> chmod

```

CHMOD(1)                  BSD General Commands Manual                 CHMOD(1)

NAME
     chmod -- change file modes or Access Control Lists

SYNOPSIS
     chmod [-fv] [-R [-H | -L | -P]] mode file ...
     chmod [-fv] [-R [-H | -L | -P]] [-a | +a | =a] ACE file ...
     chmod [-fhv] [-R [-H | -L | -P]] [-E] file ...
     chmod [-fhv] [-R [-H | -L | -P]] [-C] file ...
     chmod [-fhv] [-R [-H | -L | -P]] [-N] file ...

DESCRIPTION
     The chmod utility modifies the file mode bits of the listed files as
     specified by the mode operand. It may also be used to modify the Access
     Control Lists (ACLs) associated with the listed files.

```


> chown

```
CHOWN(8)                  BSD System Manager's Manual                 CHOWN(8)

NAME
     chown -- change file owner and group

SYNOPSIS
     chown [-fhv] [-R [-H | -L | -P]] owner[:group] file ...
     chown [-fhv] [-R [-H | -L | -P]] :group file ...

DESCRIPTION
     The chown utility changes the user ID and/or the group ID of the speci-
     fied files.  Symbolic links named by arguments are silently left
     unchanged unless -h is used.

```



