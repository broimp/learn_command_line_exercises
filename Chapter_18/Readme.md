#### Chapter_18 grep

> Show me the lines in foo.txt that have "ERROR" in them.

```
Brookss-MBP:foo $ cat foo.txt | grep -n error
1:error 1
2:error 2
```

> Show me the lines in bar.txt that have "davinci" in them.

```
Brookss-MBP:tmp $ cat bar.txt | grep -n Davinci
1:This Davinci class is fun
```

> Can you print all the lines in text files that have your first and last name in them?

```
Brookss-MBP:tmp $ grep -n Brooks my_name.txt | grep Imperial
3:Brooks Imperial

(master) Brooks Imperial
Brookss-MBP:tmp $ cat -n my_name.txt
     1	Brooks
     2	Imperial
     3	Brooks Imperial
```

$ cd temp
$ cat > newfile.txt
This is a new file.
This is a new file.
This is a new file.
$ cat > oldfile.txt
This is a old file.
This is a old file.
This is a old file.

```
(master) Brooks Imperial
Brookss-MBP:tmp $ cat > newfile.txt
This is a new file
This is a new file
This is a new file
^D
(master) Brooks Imperial
Brookss-MBP:tmp $ cat > oldfile.txt
This is an old file
This is an old file
This is an old file
```

$ grep new *.txt
newfile.txt:This is a new file.
newfile.txt:This is a new file.
newfile.txt:This is a new file.
$ grep old *.txt
oldfile.txt:This is a old file.
oldfile.txt:This is a old file.
oldfile.txt:This is a old file.
$ grep file *.txt
newfile.txt:This is a new file.
newfile.txt:This is a new file.
newfile.txt:This is a new file.
oldfile.txt:This is a old file.
oldfile.txt:This is a old file.
oldfile.txt:This is a old file.
$

```
(master) Brooks Imperial
Brookss-MBP:tmp $ grep new *.txt
another.txt:I am a new file.
ex15.txt:I am a new file.
newfile.txt:This is a new file
newfile.txt:This is a new file
newfile.txt:This is a new file

(master) Brooks Imperial
Brookss-MBP:tmp $ grep old *.txt
oldfile.txt:This is an old file
oldfile.txt:This is an old file
oldfile.txt:This is an old file

(master) Brooks Imperial
Brookss-MBP:tmp $ grep file *.txt
another.txt:I am a new file.
ex15.txt:I am a new file.
newfile.txt:This is a new file
newfile.txt:This is a new file
newfile.txt:This is a new file
oldfile.txt:This is an old file
oldfile.txt:This is an old file
oldfile.txt:This is an old file
```


> Use quotes to find "new file" and "old file" and "This is".

```
(master) Brooks Imperial
Brookss-MBP:tmp $ grep "new file" ./*
./another.txt:I am a new file.
./ex15.txt:I am a new file.
grep: ./foo: Is a directory
./newfile.txt:This is a new file
./newfile.txt:This is a new file
./newfile.txt:This is a new file

(master) Brooks Imperial
Brookss-MBP:tmp $ grep "old file" ./*
grep: ./foo: Is a directory
./oldfile.txt:This is an old file
./oldfile.txt:This is an old file
./oldfile.txt:This is an old file

(master) Brooks Imperial
Brookss-MBP:tmp $ grep "This is" ./*
grep: ./foo: Is a directory
./newfile.txt:This is a new file
./newfile.txt:This is a new file
./newfile.txt:This is a new file
./oldfile.txt:This is an old file
./oldfile.txt:This is an old file
./oldfile.txt:This is an old file
```

> Take the list of videos you created (or any other list) and use it to find some videos you want to find.

```
(master) Brooks Imperial
Brookss-MBP:tmp $ grep intro all_videos.txt
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/anki_intro_posse_cup.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/building_your_brand_wordpress_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/intro_to_agile.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/lrthw_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/mentorship_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/pivotal_tracker_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/rescuetime_and_slack_intros.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/screen_hero_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/toolbelt_intro.mp4
``` 

> Unix: You can use -i to ignore case with grep. Try grep -i new *.txt

```
(master) Brooks Imperial
Brookss-MBP:tmp $ grep -i new *.txt
another.txt:I am a new file.
ex15.txt:I am a new file.
newfile.txt:This is a new file
newfile.txt:This is a new file
newfile.txt:This is a new file
```

