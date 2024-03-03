# OTHER LANGUAGES
[Русский (Russian)](https://github.com/sapbotgit/RussianTranslations/blob/main/MiSTer-SD-Card.md)
# HOW-TO

* You need 64bit Windows 10.
* Unpack archive (release_XXXXXXXX.rar) of desired version into separate folder.
* insert SD card (you can use USB card reader)
* run MiSTer SD Card Utility.exe

Don't forget to update [MiSTer](https://github.com/MiSTer-devel/Main_MiSTer/tree/master/releases) and [Menu.rbf](https://github.com/MiSTer-devel/Menu_MiSTer/tree/master/releases) binaries on FAT partition manually (remove date-codes from names).
The versions included in this installer may be outdated!

For detailed guide [click here](https://github.com/MiSTer-devel/Wiki_MiSTer/wiki/Setup-Guide)


# New SD card layout
Starting from Release 20180115 new layout is used. Original layout had 3 partitions listed in reversed order
for windows compatibility with dedicated partition for Linux. New layout uses only 2 partitions with natural order
providing maximum compatibilty to 3rd party disk tools. Partitions won't be messed as in old format after such tools.
Linux uses image on FAT partition and thus doesn't occupy separate partition. It allows easier Linux update which needs a simple
file copy. It doesn't require reservation of SD space, thus it's only 200MB file instead of 500MB dedicated partition.

New SD installer tool and Linux supplied in new releases are backward compatible with old layout. You can continue to use the same SD card
without re-formatting. Since new version doesn't use dedicated Linux partition, the space occupied by this partition will be eventually
wasted. It's recommended to backup all your files from SD card and re-format it to new layout.

Although new SD installation tool has been tested, it still needs field testing and may have bugs. So, make a backup of your files.
