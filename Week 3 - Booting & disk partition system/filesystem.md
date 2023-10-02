# Week 3 - Booting & disk partition system

### General Boot Process
1. Power On
2. POST Process ( Pre - Operating System Test ) dilakukan oleh firmware motherboard ( BIOS )
    * saat warm booting hanya mengecek sebagian saja karena sudah di cek keseluruhan saat Cold Booting.
3. Boot

### Booting Mode
1. UEFI BIOS
    * Menggunakan partisi sistem EFI (FAT32)
    * ada Secure Boot
    * Fallback to MBR as compability Support 
2. Legacy BIOS
    * Menggunakan MBR untuk boot
    * Kebanyakan OS bisa support menggunakan ini
    * berjalan diatas CPU langsung (Real Mode)

### Disk Partition Table System
1. MBR ( Master Boot Record)
2. GPT (GUID Partition)

### Fun Fact
* Cold Booting : Proses Booting saat menyalakan komputer dari awal
* Warm Booting : Proses Booting pada saat restart komputer (menyala)
* Booting komputer server jauh lebih lama dikarenakan firmware motherboard lebih berat dan fitur yang banyak
* IPMI Protocol


