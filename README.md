Bash completion scripts for ok
=====
This repo provides bash completion for [the ok client](https://github.com/Cal-CS-61A-Staff/ok-client).

# Installation
1. Clone this repository

2-A. Register completion in your `.bashrc` like this:
```
. /path/to/repo/ok_completion
```

2-B. Or, make a link to `ok_completion` in `/etc/bash_completion.d/`.
The command should be like this:
```
$ ln /path/to/repo/ok_completion /etc/bash_completion.d
```

3. Restart your terminal.

# Usage
In your lab directory, type `python3 ok -q` and press [TAB] twice.
The console will show all available questions for the lab.

This script also completes the name of functions you want to test.
Let's say `lab01` has test cases for following questions:
 + both_positive 
 + double_eights
 
If you type `python3 ok -q b` and press [TAB], the shell will automatically replace `b` with `both_positive`.

*WARNING*: current completion is a little bit slow, please be patient.

# License
Apache License 2.0. For details, see [LICENSE](LICENSE).
