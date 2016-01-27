# RAID

> What raid level to use? And what FS?
> tl;dr Brtfs + RAID1(0)

## Choices of FS:s:

+ Brtfs (RAID0, 1, 10 - NOT 5 and 6 yet)
+ ZFS (RAID0, 1, 5, 6 1+0, 5+0, 6+0)

Comparisons:
+ http://drdabbles.us/journal/2014/2/15/my-case-for-btrfs-over-zfs.html
+ http://arstechnica.com/information-technology/2014/01/bitrot-and-atomic-cows-inside-next-gen-filesystems/1/
+ https://www.diva-portal.org/smash/get/diva2:822493/FULLTEXT01.pdf
+ http://marc.merlins.org/linux/talks/Btrfs-LinuxCon2014/Btrfs.pdf

## Choices of RAID level:

See: https://en.wikipedia.org/wiki/Standard_RAID_levels

+ RAID 0 - no redundancy, double capacity.
> Not an option!
+ RAID 1 - 1:1 redundancy, used in centrilnas 1.0.
> A likely choice.
+ RAID 10 - striped of mirrors.

## Firmware based raid?

No. Use SW RAID instead - Brtfs is SW raid.
