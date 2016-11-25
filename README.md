# Multi Ping
Ping multiple hosts and/or IPs in one window.

## Requirements
1. UNIX based system.
2. Python 3.4 or higher.

## Usage
```
usage: multiping [-h] (--host [HOST [HOST ...]] | --host-file FILE)
                 [extra [extra ...]]

Ping multiple hosts and/or IP in one window.

optional arguments:
  -h, --help            show this help message and exit
  --host [HOST [HOST ...]]
                        host to ping
  --host-file FILE      file contains hosts, one host per line

Any extra arguments will be passed to each ping task.
```

## Example
`multiping --host localhost 8.8.8.8 foo.bar -i 0.1 -c 20`↓  
![](https://raw.githubusercontent.com/eric6356/multiping/master/media/multiping.gif)

`multiping --host-file vultr-hosts.txt -i 0.1`↓  
![](https://raw.githubusercontent.com/eric6356/multiping/master/media/multiping-file.gif)
