# Usage

```bash
range 'expr'
range --list 'expr'
range --count 'expr'
range --help
```

# Options

> --list   Print range as a random list.  
> --count  Print number of item.  
> --help   Print help message.  
> 
> Print a range expression when not use option.

# Example

```bash
$ ./range 'host1.example.com,host2.example.com,host3.example.com'
host{1~3}.example.com
$ ./range -l 'host{1~3}.example.com'
host2.example.com
host3.example.com
host1.example.com
$ ./range -c 'host{1~3}.example.com'
3
```
