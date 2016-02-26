#### Chapter 14 rm

> Set up ./tmp space for practice

```
Brookss-MBP:Chapter_14 $ tree -f
.
├── ./Readme.md
└── ./tmp
    ├── ./tmp/blah.txt
    ├── ./tmp/development.log
    ├── ./tmp/foo
    │   └── ./tmp/foo/foo.txt
    ├── ./tmp/iamcool.txt
    ├── ./tmp/neat.txt
    ├── ./tmp/something
    │   └── ./tmp/something/awesome.txt
    ├── ./tmp/thefourthfile.txt
    └── ./tmp/uncool.txt

3 directories, 9 files
```

> Can you remove blah.txt?

```
Brookss-MBP:Chapter_14 $ rm ./tmp/blah.txt
```

> Let's get rid of our development log file.

```
Brookss-MBP:Chapter_14 $ rm ./tmp/development.log
```

> Can you remove everything in the slash temp slash foo directory?

```
Brookss-MBP:Chapter_14 $ rm ./tmp/foo/*
```

> DANGER: Why is it dangerous to run "rm -rf /". DO NOT RUN THIS COMMAND.
> Simply explain in the Readme.md why it's a very bad idea..

```
This comman wipes the entire hard drive on the computer. It removes all 
files and directories starting at the root director "/". It's a bad
idea because it renders the computer unusable without a complete restore.
```

> ./tmp space status after above removes, before continuing...

```
Brookss-MBP:Chapter_14 $ tree -f
.
├── ./Readme.md
└── ./tmp
    ├── ./tmp/foo
    ├── ./tmp/iamcool.txt
    ├── ./tmp/neat.txt
    ├── ./tmp/something
    │   └── ./tmp/something/awesome.txt
    ├── ./tmp/thefourthfile.txt
    └── ./tmp/uncool.txt
```    

> $ rm uncool.txt

```
Brookss-MBP:Chapter_14 $ rm ./tmp/uncool.txt
```

> $ rm iamcool.txt neat.txt thefourthfile.txt

```
Brookss-MBP:Chapter_14 $ rm ./tmp/iamcool.txt ./tmp/neat.txt ./tmp/thefourthfile.txt
```

> $ cp -r something newplace

```
Brookss-MBP:Chapter_14 $ cp -r ./tmp/something ./tmp/newplace

(master) Brooks Imperial
Brookss-MBP:Chapter_14 $ tree
.
├── Readme.md
└── tmp
    ├── foo
    ├── newplace
    │   └── awesome.txt
    └── something
        └── awesome.txt

4 directories, 3 files
```

> $ rm something/awesome.txt

```
Brookss-MBP:Chapter_14 $ rm ./tmp/something/awesome.txt
```

> $ rmdir something

```
Brookss-MBP:Chapter_14 $ rmdir ./tmp/something
```

> $ rm -rf newplace

```
Brookss-MBP:Chapter_14 $ tree
.
├── Readme.md
└── tmp
    ├── foo
    └── newplace
        └── awesome.txt

3 directories, 2 files

(master) Brooks Imperial
Brookss-MBP:Chapter_14 $ rm -rf ./tmp/newplace

(master) Brooks Imperial
Brookss-MBP:Chapter_14 $ tree
.
├── Readme.md
└── tmp
    └── foo

2 directories, 1 file
```
