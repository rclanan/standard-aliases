Standard Aliases
================

Make Linux more user friendly with this collection of (Bash aliases)(http://tldp.org/LDP/abs/html/aliases.html).

Technically they are not aliases but Bash functions, but standard aliases sounds less generic then standard functions...

This collection provides the commands, that should be in Linux by default,
or just an abveriatons of commands that are provided, but are so commonly used that they deserve a shorter name.

Bash aliases are most useful device for customizing your Linux...
Here is a short list of ones I find most useful:





Every alias that doesen't just define a different name for a command is defined as a function with descriptive name. This function is then aliased with a shorher and more convinient name. Do not change the names of the functions because they may be used by other functions.

Also only aliases get documented by generate-readme script.

By convention a function that calls the a command with some set of options that are quiet sensible for that command to be run with is named <command-name>WithSensibleOptions. This function is then usualy aliased with <command-name>1, and often also with a two letter aberration.

[**LIST OF ALL FUNCTIONS**](FUNCTION_DESCRIPTIONS.md)

Commands
--------

####  Less 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**m** | `___printOrDispl`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L63-L65) | Print or display text in pager.

####  Ls 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**l** | `___displayOutpu`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L172-L175) | List or display directory contents in pager using short listing format.

####  Tree 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**t, tree1** | `tree -C -I .git`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L264-L266) | Print directory structure.

####  Files 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**cpdir** | `cp --interactiv`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L349-L351) | Copy directories safely.
**mvdir** | `mv --interactiv`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L355-L357) | Move directories safely.
**rmdir** | `rm --interactiv`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L362-L364) | Delete directories safely.
**mk, md, mkdir1** | `mkdir --parents`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L368-L371) | Create directory and descend into.
**bk, backup** | `sudo cp --prese`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L375-L377) | Backup file.

####  Echo 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**e** | `echo "$@"` | Print text.

####  Run In Background 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**rb, runInBackground** | `nohup "$@" &>/d`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L429-L431) | Run command in background.

####  Basics 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**c** | `cat "$@"` | Print file contents.
**?, exitCode** | `echo $?` | Print exit code of last command.
**q** | `exit` | Exit bash shell.
**o, openFile** | `__runCommandInB`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L492-L494) | Open file with default app.
**te, terminal** | `gnome-terminal `[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L497-L499) | Open new terminal with same working directory.
**me, makeExecutable** | `if [[ ! -f "$1"`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L535-L564) | Make file executable or create new bash or python script.

####  Text Editors 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**v** | `vim -p "$@"` | Edit file with vim.
**vv** | `view -p "$@"` | View file in vim.

####  Sudo 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**f, fu, fuck** | `sudo $(history `[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L640-L642) | Execute last command as super user.
**sv** | `sudo vim -p "$@`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L688-L690) | Edit file with vim as super user.

####  Search 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**gr** | `__printLinesCon`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L928-L931) | Print or display with pager lines containing pattern.
**grr** | `__printLinesCon`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L935-L941) | Print or display with pager lines containing pattern in working and subdirectories.
**lo, locate1** | `locate  "$1" \`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L945-L949) | Locate files on filesystem containing pattern in their names.

####  Archives 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**extract** | `if [ -z "$1" ];`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L968-L1001) | Extract archive of any type.

####  System Information 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**df1** | `df -h | grep "s`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1029-L1031) | Print available disk space in simplified form.
**du1** | `du --summarize `[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1035-L1037) | Print disk space occupied by file or folder.

####  Misc 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**blue** | `echo -en "\e]PC`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1127-L1129) | Change hue of color blue in linux terminal.

####  Package Management 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**ch, canhaz** | `sudo apt-get in`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1177-L1179) | Install package.

####  Package Information 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------

####  Package Search 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**wi, whatis1** | `# Checks if it `[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1395-L1419) | Describe package or command or find available packages with part of name or available packages that provide command.

####  Git 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**gs** | `git -c color.st`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1471-L1474) | Print short repository status.
**gl** | `git log --decor`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1478-L1480) | Display log of commits.
**gd** | `git diff "$@"` | Display changes between commits.
**ga** | `git add "$@"` | Add files to repository.

####  Github 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**clone** | `git clone git@g`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1529-L1531) | Clone github project.

####  Network 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**ip1** | `/sbin/ifconfig `[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1562-L1568) | Print internal ip.
**pa, pingAll** | `ping -c 1 -q $(`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1589-L1593) | Ping gateway and google.
**ne, network** | `localIp=$(ip1)`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1641-L1672) | Print ssh port status of local devices and ping google.

####  Wireless 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**wr** | `woff`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1696-L1699) | Reset wireless device.

####  Internet 

 _Name_        | _Runs_   | _Description_  
:------------- |:--------:| ----------------
**i, www, internet** | `__runCommandInB`[**`...`**](https://github.com/gto76/standard-aliases/blob/master/functions#L1730-L1732) | Start default browser in background.

This aliases were made for debian based linux (ubuntu, mint,...) with gnome desktop environment, but most aliases will work on all systems with bash shell.

Most aliases will send output to pager if it will be too long to fit the screen.

Some aliases require special tools that are not installed by default on most systems. You can install them all at one with command belove, but it is probably more reasonable to just install them when demand arises.

Usualy if alias only makes command easier to use, either by providing the options that should have been set by default, or just by sending output of command to pager if necesary, then it has same name as command, but with number 1 apended at the end. Some examples are:
ps1
pgrep1
tree1
mkdir1

Only aliases that override the commands are cp, mv and rm. They are all run in interactive mode, meaning you get asked for conformation before any destructive operation. If you want to execute them without this promptint, then use -f (force) option. 

If the list belowe seems too long here is a shorthened list of aliases, that I consider almost necesary:)
m
l/ll/lll
cpdir/mvdir/rmdir
rb
o
ty
te
(ma)
mk


When adding new alias alwalys check if it is already taken by any command with `wi <alias>`.

Do not change the names of the functions, because other functions and/or aliases may be using it. You can however freely change the names of the aliases.


// Intentions
I know it is a bit abnockuous to think your colection of aliases is so great, that it should become adopted as standard, but what a hack, I worked on and been using them for long time, and I just feel so limited withouth them.


completions...
automatioc completions from the command that gets parameters in function.

Linux for the rest of us.

Linux is elegant and concise, but it is also hard.
If you can't type well and/or have problem with memorizing stuff you're basically screwed.

Make install ask you automaticaly if you want make installed, and inform you about already defined aliases (and commnet those out)
