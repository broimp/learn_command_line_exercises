#### Chapter_16 wildcard

> Can you output all the txt files in this directory?

```
Brookss-MacBook-Pro:tmp $ ls *.txt
another.txt bar.txt     ex12.txt    ex13.txt    ex15.txt    foo.txt
```

> Show me the content of the text files in slash temp.

```
Brookss-MacBook-Pro:tmp $ cat *.txt
I am a new file.
This class is fun
Hi there this is cool.
I am a fun guy.
Don't you know why?
Because I make poems,
that make babies cry.
I am a new file.
Oh so much fun
```

> $ cd temp
> $ ls *.txt

```
Brookss-MacBook-Pro:tmp $ ls *.txt
another.txt bar.txt     ex12.txt    ex13.txt    ex15.txt    foo.txt
```

> $ ls ex*.*

```
Brookss-MacBook-Pro:tmp $ ls ex*.*
ex12.txt ex13.txt ex15.txt
```

> $ ls e*

```
Brookss-MacBook-Pro:tmp $ ls e*
ex12.txt ex13.txt ex15.txt
```

> $ ls *t

```
Brookss-MacBook-Pro:tmp $ ls *t
another.txt bar.txt     ex12.txt    ex13.txt    ex15.txt    foo.txt
```

> $ cat *.txt > bigfile.txt

```
Brookss-MacBook-Pro:tmp $ cat *.txt > bigfile.txt

Brookss-MacBook-Pro:tmp $ cat bigfile.txt
I am a new file.
This class is fun
Hi there this is cool.
I am a fun guy.
Don't you know why?
Because I make poems,
that make babies cry.
I am a new file.
Oh so much fun
```

> $ rm *.txt

```
Brookss-MacBook-Pro:tmp $ rm *.txt

(master) Brooks Imperial
Brookss-MacBook-Pro:tmp $ ls

```
