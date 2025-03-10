# Booting Sequence / Booting Proce

Power On -> BIOS / UEFI -> Bootloader[first stage] -> Bootloader[Secound Stage] ->  GRUB -> Kernel -> init

# BIOS / UEFI 

##### Bios -> Basic input output software , Making initialization to the to Provide Runtime Services For operating Systems 

Intermediate way between the Hardware and OS , the BIOS use MBR [Master Boot Record] For First stage Bootloader , [post - load] process done by BIOS - POST -> power on self test [ checking for the hardware]

##### UEFI -> Unified extensible firmware interfaces , [enhancement [fasterbootime , Secure boot shell]]
        

# Firststage Bootloader

The first Stage Bootloader is Very small size  just 512 Byte The Bios Take it from [HDD / SDD / USB] and Transfer image to the RAM to [run]  and resides beside the MBR [Master Boot Record] 

# Bootloader Execution

After the BIOS / UEFI  are been executed  and initialized the hardware they  Start to look for the bootloader , in tradition BIOS , this is typicaly the MBR , In the UEFI this is ESP [ESF system Partition]
Bootloader

##### Types of BOOTLOADERS ::

1 - GRUB - Linux Common Bootloader 

2 - NLDR - Used by Older vesrion of Windows

3- BOOTMGR - used by newest version of Windows

#### Procedure 
MBR/ESP -> GRUB/Bootloader -> Kernel


# Kernel Loading


After the Bootloader is Executed , it loads the OS kernel into memory , the kernel is the core component of the OS , Manage the system , hardware , instructions
Kernel Parameters - bassed via CPU parameters , The system call is the Way Between the Kernel and UserSpace
Bootloader - Kernel 


# System Init.

#### The init process
1-Init  is the first process done by linux kernel which has PID = 1


2-it responsibel for init the system and managing the resource


3- Historically linux used the [### Sysvint system ] , which related on Shell Scripts 



