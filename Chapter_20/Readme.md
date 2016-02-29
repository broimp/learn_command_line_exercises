#### Chapter_20 apropos 

> apropos(1)                                                              apropos(1)
> 
> NAME
>        apropos - search the whatis database for strings
> 
> SYNOPSIS
>        apropos keyword ...
> 
> DESCRIPTION
>        apropos  searches  a set of database files containing short descriptions of
>        system commands for keywords and displays the result on the  standard  out-
>        put.
> 
> AUTHOR
>        John  W.  Eaton was the original author of man.  Zeyd M. Ben-Halim released
>        man 1.2, and Andries Brouwer followed up with versions 1.3 thru 1.5p.  Fed-
>        erico Lucifredi <flucifredi@acm.org> is the current maintainer.
> 
> SEE ALSO
>        whatis(1), man(1).
> 
>                                 September 19, 2005                      apropos(1)
> (END)

> Brookss-MBP:Chapter_20 $ apropos search | head

```
git-bisect(1)            - Use binary search to find the commit that introduced a bug
CPANPLUS::Internals::Search(3pm) - internals for searching for modules
DBIx::Class::CDBICompat::AbstractSearch(3pm) - Emulates Class::DBI::AbstractSearch
DBIx::Class::CDBICompat::Iterator(3pm) - Emulates the extra behaviors of the Class::DBI search iterator
NSStartSearchPathEnumeration(3), NSGetNextSearchPathEnumeration(3) - Enumeration of the filesystem paths for the various standard system directories where apps, resources, etc. get installed
Net::LDAP::Control::PersistentSearch(3pm) - LDAPv3 Persistent Search control object
Net::LDAP::Reference(3pm) - search reference
Net::LDAP::Search(3pm)   - Object returned by Net::LDAP search method
Pod::Simple::Search(3pm) - find POD documents in directory trees
Search::Dict(3pm)        - look - search for key in dictionary file
...
```

> Brookss-MBP:Chapter_20 $ apropos find | head

```
git-bisect(1)            - Use binary search to find the commit that introduced a bug
git-cherry(1)            - Find commits yet to be applied to upstream
git-merge-base(1)        - Find as good common ancestors as possible for a merge
git-name-rev(1)          - Find symbolic names for given revs
git-pack-redundant(1)    - Find redundant pack files
BIO_find_type(3ssl), BIO_next(3ssl) - BIO chain traversal
Devel::InnerPackage(3pm) - find all the inner packages of a package
File::Find(3pm)          - Traverse a directory tree
File::Find::Rule(3pm)    - Alternative interface to File::Find
File::Find::Rule::Extending(3pm) - the mini-guide to extending File::Find::Rule
...
```

> Brookss-MBP:Chapter_20 $ apropos remove | head

```
git-clean(1)             - Remove untracked files from the working tree
git-prune-packed(1)      - Remove extra objects that are already in pack files
git-rm(1)                - Remove files from the working tree and from the index
git-stripspace(1)        - Remove unnecessary whitespace
BIO_push(3ssl), BIO_pop(3ssl) - add and remove BIOs from a chain
DBIx::Class::Storage::DBI::ADO::Microsoft_SQL_Server::Cursor(3pm) - Remove trailing 
NULLs in binary data and normalize GUIDs for MSSQL over ADO
ERR_remove_state(3ssl)   - free a thread's error queue
File::Path(3pm)          - Create or remove directory trees
File::Remove(3pm)        - Remove files and directories
SLIST_EMPTY(3), SLIST_ENTRY(3), SLIST_FIRST(3), SLIST_FOREACH(3), SLIST_FOREACH_SAFE(3),
SLIST_HEAD(3), SLIST_HEAD_INITIALIZER(3), SLIST_INIT(3), SLIST_INSERT_AFTER(3), SLIST_INSERT_HEAD(3), 
SLIST_NEXT(3), SLIST_REMOVE_HEAD(3), SLIST_REMOVE(3), STAILQ_CONCAT(3), STAILQ_EMPTY(3), 
STAILQ_ENTRY(3), STAILQ_FIRST(3), STAILQ_FOREACH(3), STAILQ_FOREACH_SAFE(3), STAILQ_HEAD(3),
STAILQ_HEAD_INITIALIZER(3), STAILQ_INIT(3), STAILQ_INSERT_AFTER(3), STAILQ_INSERT_HEAD(3),
STAILQ_INSERT_TAIL(3), STAILQ_LAST(3), STAILQ_NEXT(3), STAILQ_REMOVE_HEAD(3), STAILQ_REMOVE(3),
LIST_EMPTY(3), LIST_ENTRY(3), LIST_FIRST(3), LIST_FOREACH(3), LIST_FOREACH_SAFE(3), LIST_HEAD(3), 
LIST_HEAD_INITIALIZER(3), LIST_INIT(3), LIST_INSERT_AFTER(3), LIST_INSERT_BEFORE(3),
LIST_INSERT_HEAD(3), LIST_NEXT(3), LIST_REMOVE(3), TAILQ_CONCAT(3), TAILQ_EMPTY(3), TAILQ_ENTRY(3), 
TAILQ_FIRST(3), TAILQ_FOREACH(3), TAILQ_FOREACH_SAFE(3), TAILQ_FOREACH_REVERSE(3), 
TAILQ_FOREACH_REVERSE_SAFE(3), TAILQ_HEAD(3), TAILQ_HEAD_INITIALIZER(3), TAILQ_INIT(3),
TAILQ_INSERT_AFTER(3), TAILQ_INSERT_BEFORE(3), TAILQ_INSERT_HEAD(3), TAILQ_INSERT_TAIL(3), 
TAILQ_LAST(3), TAILQ_NEXT(3), TAILQ_PREV(3), TAILQ_REMOVE(3) - implementations of
singly-linked lists, singly-linked tail queues, lists and tail queues
...
```

> Brookss-MBP:Chapter_20 $ apropos directory | head

```
git-clone(1)             - Clone a repository into a new directory
git-mv(1)                - Move or rename a file, a directory, or a symlink
git-stash(1)             - Stash the changes in a dirty working directory away
CPAN::HandleConfig(3pm)  - internal configuration handling for CPAN.pm n .SS 
"""CLASS->safe_quote ITEM""" .SS "CLASS->safe_quote ITEM" Subsection "CLASS->safe_quote ITEM" 
Quotes an item to become safe against spaces in shell interpolation. An item is enclosed in 
double quotes if:   - the item contains spaces in the middle   - the item does not start with a 
quote This happens to avoid shell interpolation problems when whitespace is present in directory 
names. This method uses commands_quote to determine the correct quote. If commands_quote is a space, 
no quoting will take place. if it starts and ends with the same quote character: leave it as it 
is if it contains no whitespace: leave it as it is if it contains whitespace, then if it contains 
quotes: better leave it as it is else: quote it with the correct quote type for the box we're on
CPANPLUS::Internals::Source::Memory(3pm) - In memory implementation n .SS 
"$cb->_|_memory_retrieve_source(name => $name, [path => $path, uptodate => BOOL, verbose => BOOL])" 
.SS "$cb->_|_memory_retrieve_source(name => $name, [path => $path, uptodate => BOOL, verbose => BOOL])" 
Subsection "$cb->__memory_retrieve_source(name => $name, [path => $path, uptodate => BOOL, 
verbose => BOOL])" This method retrieves a storabled tree identified by $name. It takes the following 
arguments: name" 4 Item "name" The internal name for the source file to retrieve. uptodate" 4 Item 
"uptodate" A flag indicating whether the file-cache is up-to-date or not. path" 4 Item "path" The 
absolute path to the directory holding the source files. verbose" 4 Item "verbose" A boolean flag 
indicating whether or not to be verbose. Will get information from the config file by default. 
Returns a tree on success, false on failure. n .SS "$cb->_|_memory_save_source([verbose => BOOL, 
path => $path])" .SS "$cb->_|_memory_save_source([verbose => BOOL, path => $path])" Subsection 
"$cb->__memory_save_source([verbose => BOOL, path => $path])" This method saves all the parsed 
trees in storabled format if Storable is available. It takes the following arguments: path" 4 
Item "path" The absolute path to the directory holding the source files. verbose" 4 Item "verbose" 
A boolean flag indicating whether or not to be verbose. Will get information from the config file 
by default. Returns true on success, false on failure
CURLOPT_CAPATH(3)        - specify directory holding CA certificates
CURLOPT_DIRLISTONLY(3)   - ask for names only in a directory listing
CURLOPT_FTP_FILEMETHOD(3) - select directory traversing method for FTP
CURLOPT_NEW_DIRECTORY_PERMS(3) - permissions for remotely created directories
CURLOPT_WILDCARDMATCH(3) - enable directory wildcard transfers
...
```
