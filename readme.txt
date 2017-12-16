Last login: Sat Dec 16 13:11:46 on ttys001
luansggdeMacBook-Pro:gittest luan$ git commit -m 'initial project version'
[master (root-commit) ed64786] initial project version
 Committer: luansgg <luan@luansggdeMacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 111 insertions(+)
 create mode 100644 index.php
luansggdeMacBook-Pro:gittest luan$ git config --global
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)

luansggdeMacBook-Pro:gittest luan$ git config --global --local
error: only one config file at a time.
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)

luansggdeMacBook-Pro:gittest luan$ git config --global --get
error: wrong number of arguments
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)

luansggdeMacBook-Pro:gittest luan$ https://github.com/luangg/laravel0.git
-bash: https://github.com/luangg/laravel0.git: No such file or directory
luansggdeMacBook-Pro:gittest luan$ git clone https://github.com/luangg/laravel0.git
Cloning into 'laravel0'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
luansggdeMacBook-Pro:gittest luan$ git clone https://github.com/luangg/laravel0.git newname
Cloning into 'newname'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
luansggdeMacBook-Pro:gittest luan$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	laravel0/
	newname/

nothing added to commit but untracked files present (use "git add" to track)
luansggdeMacBook-Pro:gittest luan$ cd newname
luansggdeMacBook-Pro:newname luan$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
luansggdeMacBook-Pro:newname luan$ vim readme

this is a readme file !

~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
~                                                                                                                                                                                                           
-- INSERT --
