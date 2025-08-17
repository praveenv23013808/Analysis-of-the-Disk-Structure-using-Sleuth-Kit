# Analysis-of-the-Disk-Structure-using-Sleuth-Kit

## AIM:

To analyze the disk structure of a given disk image using Sleuth Kit tools in Kali Linux.

## DESIGN STEPS:

## Step 1:
Obtain or create a disk image file (e.g., disk.dd) to analyze. Open the terminal in Kali Linux.

## Step 2:
Use Sleuth Kit tools like mmls, fsstat, and fls to examine the partition layout, file system details, and file listing.

## Step 3:
Interpret the output of the tools to understand the disk structure, including partitions, sectors, and files.

## PROGRAM:

### Sleuth Kit Disk Analysis Commands

#### Create a Sample Disk Image (for Testing)

#### Let’s create a 10MB blank disk image and simulate file system activity:

```
cd ~/Downloads
```

#### Step 1: Create an empty disk image

```
dd if=/dev/zero of=disk.dd bs=1M count=10
```

#### Step 2: Format it with a file system (like FAT32)

```
mkfs.vfat disk.dd
```

## OUTPUT:

#### Name - Kantha Sishanth S
#### Reg. No. - 212222100020

<img width="934" height="241" alt="1" src="https://github.com/user-attachments/assets/71ebd1cd-7e5b-4112-ae29-60a6f1f0efa6" />



## Create Disk

<img width="1059" height="398" alt="2" src="https://github.com/user-attachments/assets/b90c9ab4-05ab-4d7c-a80c-d47cabfecac5" />



## mmls

```
mmls disk.dd
```

## fls

```
fls -f fat -o 0 disk.dd
```

<img width="517" height="240" alt="3" src="https://github.com/user-attachments/assets/16da78d0-8b9e-4f20-9c31-76a87b562831" />

<img width="995" height="571" alt="4" src="https://github.com/user-attachments/assets/41e6d26e-bd4b-44c7-9aec-84cb2504b251" />

<img width="569" height="183" alt="5" src="https://github.com/user-attachments/assets/03c5695b-652d-402f-95c2-519e76c58c2e" />

<img width="495" height="299" alt="6" src="https://github.com/user-attachments/assets/cc8d4164-7f2c-4edb-875e-a34640580bb6" />



## RESULT:

The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.
