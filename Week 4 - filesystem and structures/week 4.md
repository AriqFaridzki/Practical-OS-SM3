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
    * ext
        * 2GB max File and Volume size
        * 255 Character limit
    * ext2 
        * inode Concept ( index - node ) 
        * 2TB Max file Size
        * 32TB max Volume Size
    * ext3
        * Journaling support
        * Directory Index
    * ext4
        * Journal double checking (journal checksum)
        * infinity Subdirectory
        * presistent pre-allocation
        * faster filechecking
        * win & mac support (3rd party like WSL)
        * 16 TB max file size
        * 1 EB max Volume size 
2. other

### funfact
> Linking in linux : soft link, hardlink [tutorial](https://opensource.com/article/17/6/linking-linux-filesystem)

> sector size ? [tutorial ](https://www.mirazon.com/understanding-hard-disk-sector-size-part-1-the-change/)

> Journaling : is to keep track of changes not yet committed to the file system. Even after any crashes or unexpected shutdowns, you can still access the latest file version with a lower likelihood of it becoming corrupted.

