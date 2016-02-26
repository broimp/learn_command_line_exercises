#### Chapter_15 pipes and redirection

> Can you put "This class is fun" into bar.txt?

```
Brookss-MBP:Chapter_15 $ echo 'This class is fun' > ./tmp/bar.txt
```

> Can you put "Oh so much fun" into foo.txt?

```
Brookss-MBP:Chapter_15 $ echo 'Oh so much fun' > ./tmp/foo.txt
```

> Explain what the |, <, > and >> commands do in your own words

```
The pipe | operator takes the output from the left side of the pipe
and sends to the input of the command on the right side of the pipe.

The < operator routes the input from the right side of the operator
to the command on the left. It's a counter inutuitive reverse flow 
and, as a result, I expect it doesn't get used much.

The > operator routes the output from the left to the command or file 
on the right.

The >> operator appends the output from the left to the file on the
right.
```

> $ cat ex12.txt ex13.txt | less

```
Brookss-MBP:Chapter_15 $ cat ./tmp/ex12.txt ./tmp/ex13.txt | less
```

> $ cat < ex13.txt

```
Brookss-MBP:tmp $ cat < ex13.txt
I am a fun guy.
Don't you know why?
Because I make poems,
that make babies cry.
```

> $ less < ex12.txt

```
Brings up the less editor
```

> $ less < ex12.txt | cat | less

```
This command puts the ex12.txt in the less editor, but it's ambiguous
as to which less command is operating - the one on the left or the
one on the right. I wouldn't advise this command structure.
```

> $ cat ex13.txt > ex15.txt

```
Takes contents of ex13.txt and overwrites contents of ex15.txt
```

> cat ex12.txt,ex13.txt | more

```
This command fails - the comma should be a space.
```

```
Brookss-MBP:tmp $ echo "I am a new file." > ex15.txt

Brookss-MBP:tmp $ cat ex15.txt
I am a new file.

Brookss-MBP:tmp $ cat ex15.txt > another.txt

Brookss-MBP:tmp $ cat another.txt
I am a new file.

Brookss-MBP:tmp $ cat ex15.txt | more
I am a new file.
```
