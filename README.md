# terminator-split
Wrapper script for splitting Terminator terminal emulator

```shell
$ terminator-split --help
usage:
        terminator-split [-h] [-d]
                         [-e COMMAND] [-g CONFIG] [-t TERMINATOR]
                         [TERMINATOR_OPTIONS]
                         hostname [hostname ...]

        terminator-split [-h] [-d]
                         [-g CONFIG] [-t TERMINATOR] [-s SHELL]
                         [TERMINATOR_OPTIONS]
                         number


positional arguments:
  hostname

optional arguments:
  -h, --help                              show this help message and exit
  -d, --debug                             show debug messages at execution time
  -e COMMAND, --command COMMAND
  -g CONFIG, --config CONFIG              Use this terminator config file
  -s SHELL, --shell SHELL                 Specify the shell to be loaded
  -t TERMINATOR, --terminator TERMINATOR
```

```shell
terminator-split command1 command2 command3
```

Note that the username can also be specified as part of the servername. Eg:

```shell
terminator-split 'ssh user1@server1' 'ssh user2@server2 -p 500'
```

![](https://github.com/AlekseyChudov/terminator-split/blob/master/images/terminator-split-4.png?raw=true)

```shell
terminator-split 8
```

![](https://github.com/AlekseyChudov/terminator-split/blob/master/images/terminator-split-8.png?raw=true)
