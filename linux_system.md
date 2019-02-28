

# General
## Commands
### Stats
#### free

    $ free -m

To see stats about available, max, used, etc. memory of the system.

**Tags:** available, memory, ubuntu

#### parted

    $ sudo parted /dev/sda unit GB print free | grep 'Free Space' | tail -n1 | awk '{print $3}'

Check the available, unpartitioned space available on the physical disk /dev/sda. Substitute with the device name you want to check.

**Tags:** free, disk, physical, partition, space

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

An alternative for CPU infos is:

	$ lscpu
