# subc: a bash script framework



## installation

    wget https://raw.githubusercontent.com/simon/subc/master/sub -O my_script
    chmod +x my_script
    ./my_script


## example usage 

``` bash
$ ./sub
cmd1 : cmd1 is an awesome command
cmd2 : cmd2 is an more awesome command
help : display help on a command
```


## add your commands

edit your script file and replace cmd1 by your command name. 

fill also ```_USAGE``` and ```_HELP```

``` bash
_sub_cmd1(){
    _USAGE="arg1"
    _HELP="cmd1 is an awesome command"

    run(){
        echo run cmd1 -- $@
    }
}
```


