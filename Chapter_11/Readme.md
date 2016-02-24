#### Chapter_11
#### mv terminal command

> $ cd temp
> $ mv awesome.txt uncool.txt
> $ ls
> newplace    uncool.txt
> $ mv newplace oldplace
> $ ls
> oldplace    uncool.txt
> $ mv oldplace newplace
> $ ls
> newplace   uncool.txt

> Can you rename foo.txt to blah.txt?
> Can you move the production.log file in the log directory to slash temp?
> Move a file in the newplace directory to another directory then move it back.

```
Brookss-MBP:Chapter_11 $ mkdir ./tmp

Brookss-MBP:Chapter_11 $ cd tmp

Brookss-MBP:tmp $ pwd
/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_11/tmp

Brookss-MBP:tmp $ echo 'awesome' > awesome.txt

Brookss-MBP:tmp $ cat awesome.txt
awesome

Brookss-MBP:tmp $ mv awesome.txt uncool.txt

Brookss-MBP:tmp $ cat uncool.txt
awesome

Brookss-MBP:tmp $ ls -l
total 8
-rw-r--r--  1 bi  staff  8 Feb 24 12:12 uncool.txt

Brookss-MBP:tmp $ mkdir newplace

Brookss-MBP:tmp $ ls
newplace   uncool.txt

Brookss-MBP:tmp $ mv newplace oldplace

Brookss-MBP:tmp $ ls
oldplace   uncool.txt

Brookss-MBP:tmp $ mv oldplace newplace

Brookss-MBP:tmp $ ls
newplace   uncool.txt

Brookss-MBP:tmp $ echo 'foo' > foo.txt

Brookss-MBP:tmp $ mv foo.txt blah.txt

Brookss-MBP:tmp $ ls
blah.txt   newplace   uncool.txt

Brookss-MBP:tmp $ cd ..

Brookss-MBP:Chapter_11 $ echo 'production' > production.log

Brookss-MBP:Chapter_11 $ mv production.log ./tmp/

Brookss-MBP:Chapter_11 $ ls
Readme.md tmp

Brookss-MBP:Chapter_11 $ ls ./tmp
blah.txt       newplace       production.log uncool.txt

Brookss-MBP:Chapter_11 $ ls ./tmp/newplace/

Brookss-MBP:Chapter_11 $ echo 'some data' > ./tmp/newplace/some_data.txt

Brookss-MBP:Chapter_11 $ ls ./tmp/newplace/
some_data.txt

Brookss-MBP:Chapter_11 $ mv ./tmp/newplace/some_data.txt ./tmp/

Brookss-MBP:Chapter_11 $ ls ./tmp/newplace/

Brookss-MBP:Chapter_11 $ ls ./tmp
blah.txt       newplace       production.log some_data.txt  uncool.txt

Brookss-MBP:Chapter_11 $ mv ./tmp/some_data.txt ./tmp/newplace/.

Brookss-MBP:Chapter_11 $ ls ./tmp/newplace/
some_data.txt
```
