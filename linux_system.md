

# General
## Commands
### Stats
#### free

    $ free -m

To see stats about available, max, used, etc. memory of the system.

**Tags:** available, memory, ubuntu

## Files

### Stats
#### /proc/sys/fs/file-max

    $ cat /proc/sys/fs/file-max

Check the maximum allowed amount of open files systemwide.

**Tags:** max, amount, open, files, system, wide, ubuntu

**Alternative:** lsof | wc -l

# CentOS (7)
## Commands
### System Info
#### df -h && cat /proc/meminfo && cat /proc/cpuinfo

    $ df -h && cat /proc/meminfo && cat /proc/cpuinfo

Or each one by itself:

Get the hard disk usage

     $ df -h

Get the system memory info:

    $ cat /proc/meminfo

Get the CPU info:

    $ cat /proc/cpuinfo