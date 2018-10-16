# Usage

```bash
myrange 'expr'
myrange --list 'expr'
myrange --count 'expr'
myrange --help
```

# Options

> --list   Print range as a random list.  
> --count  Print number of item.  
> --help   Print help message.  
> 
> Print a range expression when not use option.

# Example

```bash
$ ./myrange 'host1.example.com,host2.example.com,host3.example.com'
host{1~3}.example.com
$ ./myrange -l 'host{1~3}.example.com'
host2.example.com
host3.example.com
host1.example.com
$ ./myrange -c 'host{1~3}.example.com'
3
```
