# 42Bangkok | Pipex, an intro to fork()

## Understand pipex

The goal of pipex is to develop a program that imitate shell's pipelines behavior, so we got to understand how pipes works in bash beforehand.

```bash
< infile cmd1 | cmd2 > outfile
```

This is regular use of pipe in shell, lets break this line down.

* ```<``` or Input redirection : This option redirects ```infile``` content into STDIN.
* ```infile``` : File that follows ```<``` option, it's content will be redirect to STDIN.
* ```cmd1``` : you could replace this with regular shell command e.g. cat grep sleep ...
* ```|``` or Pipe : This is a bridge that connect between commands, redirect output from ```cmd1``` to become an input on ```cmd2```. (It behaves this way, but it actually fast switching between commands)
* ```cmd2``` : regular shell command same as ```cmd1```.
* ```>``` or Output redirection : This option redirects an outputted result of the whole command into ```outfile```. 

