## Shell Scripting Basics
- shebang interpreter directive
- script is a list of command that can be intrepreted by scripting lang
- scripting language are interpreted at runtime
- used in automation jobs like - file archive, etl jobs, system administration jobs
- first line in a shell script is the interpreter directive; called shebang
- #!/bin/sh
- #!/bin/bash
- #!/usr/bin/env python3
- echo (prints from to ) echo >>
- $var_name to point to a variable
```
$ read lastname  
Grossman  
$ echo $lastname  
Grossman  
```
- read command stores value in next line to lastname (it lets user to input information and store in a variable)

## Filters, Pipes, and Variables
- explain pipe and filters
- shell and environment varibale
- filters are shell command which take input from default into and return output to standard output
- wc,sort,cat,more,head,grep
- value of filter can be chained together using pipe
- command1 | command2 (output of command 1 used as input of 2)
- pipe is short for pipeline
- set (command to display all shell variable)
- unset audience (delets the variable audience)
- environment variable are just like shell variable but they have extended scopes
- export var_name (make var_name environment variable)
- env to list all environemnt variable
- $ sort pets.txt | uniq (first sort then remove consecutive duplicate line)
- tr (translate) - replaces characters in input text
```
$ echo "Linux and shell scripting are awesome\!" | tr "aeiou" "_"
L_n_x _nd sh_ll scr_pt_ng _r_ _w_s_m_!
----
$ echo "Linux and shell scripting are awesome\!" | tr -c "aeiou" "_"
_i_u__a_____e______i__i___a_e_a_e_o_e_
----
$ curl -s --location --request GET https://api.coinstats.app/public/v1/coins/bitcoin\?currency\=USD |\
    grep -oE "\"price\":\s*[0-9]*?\.[0-9]*" |\
    grep -oE "[0-9]*?\.[0-9]*"
57907.78008618953
```
## Useful Features of the Bash Shell
- metacharacter is unique character
- # - comment
- ; - command separator in same line
- 
- 
