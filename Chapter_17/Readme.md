#### Chapter_17 find

> Can you show me all the files in slash temp slash foo?

```
Brookss-MacBook-Pro:tmp $ find .
.
./another.txt
./bar.txt
./ex12.txt
./ex13.txt
./ex15.txt
./foo
./foo/foo.txt
```

> What log files are in your log directory?

```
Brookss-MacBook-Pro:tmp $ find / | grep /log/ > log_files.txt
 
There are quite a few files in various log directories.
See log_files.txt
```

> $ cd temp
> $ find . -name "*.txt" -print

```
Brookss-MacBook-Pro:tmp $ find . -name "*.txt" -print
./another.txt
./bar.txt
./ex12.txt
./ex13.txt
./ex15.txt
./foo/foo.txt
./log_files.txt
```


> $ cd ..
> $ find . -name "*.txt" -print | less

```
./tmp/another.txt
./tmp/bar.txt
./tmp/ex12.txt
./tmp/ex13.txt
./tmp/ex15.txt
./tmp/foo/foo.txt
./tmp/log_files.txt
```

> $ cd ..
> $ find . -name "*.txt" -print | less

```
Brookss-MacBook-Pro:tmp $ find . -name "*.txt" -print
./another.txt
./bar.txt
./ex12.txt
./ex13.txt
./Chapter_11/tmp/blah.txt
./Chapter_11/tmp/newplace/some_data.txt
./Chapter_11/tmp/uncool.txt
./Chapter_12/tmp/ex12.txt
./Chapter_13/tmp/ex12.txt
./Chapter_13/tmp/ex13.txt
./Chapter_15/tmp/another.txt
./Chapter_15/tmp/bar.txt
./Chapter_15/tmp/ex12.txt
./Chapter_15/tmp/ex13.txt
./Chapter_15/tmp/ex15.txt
./Chapter_15/tmp/foo.txt
./Chapter_17/tmp/another.txt
./Chapter_17/tmp/bar.txt
./Chapter_17/tmp/ex12.txt
./Chapter_17/tmp/ex13.txt
./Chapter_17/tmp/ex15.txt
./Chapter_17/tmp/foo/foo.txt
./Chapter_17/tmp/log_files.txt
```

> You can put any directory where the . (dot) is. Try another directory 
> to start your search there. Look for all the video files on your
> computer starting at the home drive and use the > to save
> the list to a file. Remember how you can do SOMECOMMAND > SOMEFILE.txt
> and it will write the output of SOMECOMMAND to the file SOMEFILE.txt?

```
Brookss-MacBook-Pro:learn_command_line_exercises $ find / -name "*.mp4" -print > all_videos.txt

Brookss-MacBook-Pro:tmp $ cat all_videos.txt
/Users/bi/.rvm/src/ruby-2.2.4/sample/trick2013/mame/music-box.mp4
/Users/bi/Downloads/Git - Part 2.mp4
/Users/bi/OReilly Ed/Ruby Intro/CodeRunner Code Editor Demo.mp4
/Users/bi/OReilly Ed/Ruby Intro/CodeRunner Coursework Demo.mp4
/Users/bi/OReilly Ed/Ruby Intro/CodeRunner File Management Demo.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/git_review_with_tim/Git - Part 1.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/git_review_with_tim/Git - Part 2.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/git_review_with_tim/Git - Part 3.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/adding_tests_to_homework.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/agile_retrospective.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/anki_intro_posse_cup.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/arrays.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/building_your_brand_wordpress_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/fixing_rubocop_errors.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/git_101.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/git_101_warmup.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/git_102.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/git_branching_homework_review.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/intro_to_agile.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/learn_command_line_part_1.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/learn_command_line_part_2.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/lrthw_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/making_it_stick.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/mentorship_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/methods_and_flow_control.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/methods_and_recursion.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/numbers_letters_and_variables.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/pair_programming.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/pivotal_tracker_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/questions_gitignore_mine_autocomplete.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/random_number_guesser.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/rescuetime_and_slack_intros.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/screen_hero_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/toolbelt_intro.mp4
/Users/bi/workspace/DaVinci_videos/DaVinci_Videos_T1_2016/in_class/tracker_warmup_and_posses.mp4

(master) Brooks Imperial
```
> Run find in the class directory, pipe the output to pbcopy and create
> a gist with the content. Run find in the class directory, pipe the
> output to pbcopy and create a gist with the content.  
> Paste the Gist URL as a comment on this story.

```
https://gist.github.com/broimp/34056eea75961f95483d
```



 
