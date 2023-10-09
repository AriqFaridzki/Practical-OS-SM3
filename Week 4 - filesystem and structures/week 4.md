# Filesystem.
filesystem itu sendiri adalah bagaimana sistem itu mengatur data data yang disimpan. 

setiap filesystem itu mempunyai keunikan sendiri dalam setiap formatnya (NTFS, ext4, FAT32, dll)

## Windows Filesystem Format
1. FAT ( File Allocation Table ) : kompabilitas jauh lebih oke
    * FAT16
    * FAT32 
    * exFAT
2. NTFS (New Technology File System) : kompabilitas kepada mac sama linux agak kurang (pake 3rd party)
    * Feature :
    * Access control list
    * Journaling
    * Soft Link and Hard link support
    * 256TB max filesize ( 8tb on win 10 1709)
    * 256TB max volume size ( 8tb on win 10 1709 )
3. ReFS (Resilient File System) sama seperti NTFS tapi lebih bagus journalingnya ( kayak git tapi buat filesystem )
    * Feature
    * 16 EB Max Filesize
    * 1 YB Max Volume Size
    * Better Journaling
    * Next gen NTFS


## Linux Filesystem
1. Ext ( Extended File Format )
    * ext2 
    * ext3
    * ext4

        * Feature
        * For Linux
        * 255 Character limit
        * 
        * 
        * 
2. dll

### funfact
> Linking in linux : soft link, hardlink [tutorial](https://opensource.com/article/17/6/linking-linux-filesystem)

> sector size ? [tutorial ](https://www.mirazon.com/understanding-hard-disk-sector-size-part-1-the-change/)

> Journaling : is to keep track of changes not yet committed to the file system. Even after any crashes or unexpected shutdowns, you can still access the latest file version with a lower likelihood of it becoming corrupted.

