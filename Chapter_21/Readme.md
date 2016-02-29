#### Chapter_21 env - environment variables

$ env

```
Brookss-MBP:learn_command_line_exercises $ env
rvm_bin_path=/Users/bi/.rvm/bin
TERM_PROGRAM=iTerm.app
GEM_HOME=/Users/bi/.rvm/gems/ruby-2.2.4
TERM=xterm-256color
SHELL=/bin/bash
CLICOLOR=1
IRBRC=/Users/bi/.rvm/rubies/ruby-2.2.4/.irbrc
TMPDIR=/var/folders/j2/bw272vsj00xg8xmdfh5vbdl80000gn/T/
Apple_PubSub_Socket_Render=/private/tmp/com.apple.launchd.0p6GSpNsS1/Render
OLDPWD=/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_20
MY_RUBY_HOME=/Users/bi/.rvm/rubies/ruby-2.2.4
USER=bi
_system_type=Darwin
COMMAND_MODE=unix2003
rvm_path=/Users/bi/.rvm
SSH_AUTH_SOCK=/private/tmp/com.apple.launchd.1tlUw9x69D/Listeners
__CF_USER_TEXT_ENCODING=0x1F5:0x0:0x0
rvm_prefix=/Users/bi
PATH=/Users/bi/.rvm/gems/ruby-2.2.4/bin:/Users/bi/.rvm/gems/ruby-2.2.4@global/bin:/Users/bi/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Users/bi/.rvm/bin
PWD=/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
LANG=en_US.UTF-8
ITERM_PROFILE=Default
_system_arch=x86_64
XPC_FLAGS=0x0
_system_version=10.11
XPC_SERVICE_NAME=0
rvm_version=1.26.11 (master)
SHLVL=1
HOME=/Users/bi
COLORFGBG=12;8
ITERM_SESSION_ID=w0t0p0
LOGNAME=bi
GEM_PATH=/Users/bi/.rvm/gems/ruby-2.2.4:/Users/bi/.rvm/gems/ruby-2.2.4@global
RUBY_VERSION=ruby-2.2.4
SECURITYSESSIONID=186a8
_system_name=OSX
BASH_FUNC_parse_git_pair%%=() {  if ( hub rev-parse --git-dir > /dev/null 2>&1 ); then
 hub config user.name;
 fi
}
BASH_FUNC_parse_git_branch%%=() {  hub branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
_=/usr/bin/env
```

$ env | grep -i users

```
Brookss-MBP:learn_command_line_exercises $ env | grep -i users
rvm_bin_path=/Users/bi/.rvm/bin
GEM_HOME=/Users/bi/.rvm/gems/ruby-2.2.4
IRBRC=/Users/bi/.rvm/rubies/ruby-2.2.4/.irbrc
OLDPWD=/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises/Chapter_20
MY_RUBY_HOME=/Users/bi/.rvm/rubies/ruby-2.2.4
rvm_path=/Users/bi/.rvm
rvm_prefix=/Users/bi
PATH=/Users/bi/.rvm/gems/ruby-2.2.4/bin:/Users/bi/.rvm/gems/ruby-2.2.4@global/bin:/Users/bi/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Users/bi/.rvm/bin
PWD=/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
HOME=/Users/bi
GEM_PATH=/Users/bi/.rvm/gems/ruby-2.2.4:/Users/bi/.rvm/gems/ruby-2.2.4@global
```

> Brookss-MBP:learn_command_line_exercises $ echo $USER

```
bi
```

> Brookss-MBP:learn_command_line_exercises $ echo $PWD

```
/Users/bi/workspace/davinci_coders_t1_2016/homework/learn_command_line_exercises
```

> Brookss-MBP:learn_command_line_exercises $ export TESTING="1 2 3"

```
Brookss-MBP:learn_command_line_exercises $ echo $TESTING
1 2 3
```

> Changing the directory path

export PATH=$PATH:/usr/local/foo  (for example)

```
Brookss-MBP:learn_command_line_exercises $ echo $PATH
/Users/bi/.rvm/gems/ruby-2.2.4/bin:/Users/bi/.rvm/gems/ruby-2.2.4@global/
bin:/Users/bi/.rvm/rubies/ruby-2.2.4/bin:/usr/local/bin:/usr/bin:/
bin:/usr/sbin:/sbin:/Users/bi/.rvm/bin
```

**NOTE: I will NOT be experimenting with changing my default path at this time. There's 
too much that could go wrong and cost me hours to recover.
