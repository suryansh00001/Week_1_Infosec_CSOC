pure bash you can see


  suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file flag.pdf
    flag.pdf: shell archive text
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv flag.pdf flag.sh
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ chmod +x flag.sh
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ ./flag.sh
    x - created lock directory _sh00046.
    x - SKIPPING flag (file already exists)
    x - removed lock directory _sh00046.
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file flag
    flag: current ar archive
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ ar x flag
    ar: flag: malformed archive
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ .flag.sh
    .flag.sh: command not found
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ ./flag.sh
    x - created lock directory _sh00046.
    x - extracting flag (text)
    x - removed lock directory _sh00046.
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file flag
    flag: current ar archive
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ ar x flag
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file flag
    flag: cpio archive; device 234, inode 37426, mode 100644, uid 0, gid 0, modified Thu Mar 16 01:40:17 2023, 510 bytes "flag"
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ cpio -i <flag
    Command 'cpio' not found, but can be installed with:
    sudo apt install cpio
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ sudo apt install cpio
    Reading package lists... Done
    Building dependency tree... Done
    Reading state information... Done
    Suggested packages:
      libarchive-dev
    The following NEW packages will be installed:
      cpio
    0 upgraded, 1 newly installed, 0 to remove and 62 not upgraded.
    Need to get 82.7 kB of archives.
    After this operation, 336 kB of additional disk space will be used.
    Get:1 http://archive.ubuntu.com/ubuntu noble/main amd64 cpio amd64 2.15+dfsg-1ubuntu2 [82.7 kB]
    Fetched 82.7 kB in 2s (39.2 kB/s)
    Selecting previously unselected package cpio.
    (Reading database ... 61149 files and directories currently installed.)
    Preparing to unpack .../cpio_2.15+dfsg-1ubuntu2_amd64.deb ...
    Unpacking cpio (2.15+dfsg-1ubuntu2) ...
    Setting up cpio (2.15+dfsg-1ubuntu2) ...
    update-alternatives: using /usr/bin/mt-gnu to provide /usr/bin/mt (mt) in auto mode
    Processing triggers for man-db (2.12.0-4build2) ...
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ cpio -i <flag
    cpio: flag not created: newer or same age version exists
    2 blocks
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv flag a
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ cpio -i <a
    2 blocks
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file a
    a: cpio archive; device 234, inode 37426, mode 100644, uid 0, gid 0, modified Thu Mar 16 01:40:17 2023, 510 bytes "flag"
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file flag
    flag: bzip2 compressed data, block size = 900k
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv flag b.bzip2
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ bunzip2 b.bzip2
    bunzip2: Can't guess original name for b.bzip2 -- using b.bzip2.out
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ ls
    //// private data
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file b.bzip2.out
    b.bzip2.out: gzip compressed data, was "flag", last modified: Thu Mar 16 01:40:17 2023, from Unix, original size modulo 2^32 327
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv b
    b.bzip2.out                        boardXII_compressed.pdf            book (5).jpg
    blender-4.2.0-windows-x64.msi      boardX_compressed.pdf              book (6).jpg
    board Xii scanned (1) (1).pdf      book (1).jpg                       book.jpg
    board Xii scanned (1) (2).pdf      book (2).jpg                       branch-change-2023-list-new.pdf
    board Xii scanned (1).pdf          book (3).jpg                       brief_project_description.pdf.pdf
    board Xii scanned.pdf              book (4).jpg
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv b.bzip2.out g.gzip
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ gunzip g.gzip
    gzip: g.gzip: unknown suffix -- ignored
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g.gzip g.gz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ gunzip g.gz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: lzip compressed data, version: 1
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.lz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lunzip g.lz
    Command 'lunzip' not found, but can be installed with:
    sudo apt install lunzip
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ sudo apt install lunzip
    Reading package lists... Done
    Building dependency tree... Done
    Reading state information... Done
    The following NEW packages will be installed:
      lunzip
    0 upgraded, 1 newly installed, 0 to remove and 62 not upgraded.
    Need to get 33.9 kB of archives.
    After this operation, 85.0 kB of additional disk space will be used.
    Get:1 http://archive.ubuntu.com/ubuntu noble/universe amd64 lunzip amd64 1.14-1 [33.9 kB]
    Fetched 33.9 kB in 2s (21.5 kB/s)
    Selecting previously unselected package lunzip.
    (Reading database ... 61158 files and directories currently installed.)
    Preparing to unpack .../lunzip_1.14-1_amd64.deb ...
    Unpacking lunzip (1.14-1) ...
    Setting up lunzip (1.14-1) ...
    update-alternatives: using /usr/bin/lzip.lunzip to provide /usr/bin/lzip (lzip) in auto mode
    update-alternatives: using /usr/bin/lzip.lunzip to provide /usr/bin/lzip-decompressor (lzip-decompressor) in auto mode
    Processing triggers for man-db (2.12.0-4build2) ...
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lunzip g.lz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: LZ4 compressed data (v1.4+)
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.lz4
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lunzip4 g.lz4
    Command 'lunzip4' not found, did you mean:
      command 'lunzip' from deb lunzip (1.13-6)
    Try: sudo apt install <deb name>
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lz4 -d g.lz4
    Command 'lz4' not found, but can be installed with:
    sudo snap install lz4  # version 1.9.4, or
    sudo apt  install lz4  # version 1.9.4-1build1.1
    See 'snap info lz4' for additional versions.
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ sudo apt  install lz4  # version 1.9.4-1build1.1
    Reading package lists... Done
    Building dependency tree... Done
    Reading state information... Done
    The following NEW packages will be installed:
      lz4
    0 upgraded, 1 newly installed, 0 to remove and 62 not upgraded.
    Need to get 93.8 kB of archives.
    After this operation, 238 kB of additional disk space will be used.
    Get:1 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 lz4 amd64 1.9.4-1build1.1 [93.8 kB]
    Fetched 93.8 kB in 2s (47.0 kB/s)
    Selecting previously unselected package lz4.
    (Reading database ... 61167 files and directories currently installed.)
    Preparing to unpack .../lz4_1.9.4-1build1.1_amd64.deb ...
    Unpacking lz4 (1.9.4-1build1.1) ...
    Setting up lz4 (1.9.4-1build1.1) ...
    Processing triggers for man-db (2.12.0-4build2) ...
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lz4 -d g.lz4
    Decoding file g
    g.lz4                : decoded 265 bytes
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: LZMA compressed data, non-streamed, size 254
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.lzma
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ xz -d g.lzma
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: lzop compressed data - version 1.040, LZO1X-1, os: Unix
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.lzo
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lzop -d g.lzo
    Command 'lzop' not found, but can be installed with:
    sudo apt install lzop
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ sudo apt install lzop
    Reading package lists... Done
    Building dependency tree... Done
    Reading state information... Done
    The following NEW packages will be installed:
      lzop
    0 upgraded, 1 newly installed, 0 to remove and 62 not upgraded.
    Need to get 82.2 kB of archives.
    After this operation, 161 kB of additional disk space will be used.
    Get:1 http://archive.ubuntu.com/ubuntu noble/main amd64 lzop amd64 1.04-2build3 [82.2 kB]
    Fetched 82.2 kB in 1s (55.5 kB/s)
    Selecting previously unselected package lzop.
    (Reading database ... 61178 files and directories currently installed.)
    Preparing to unpack .../lzop_1.04-2build3_amd64.deb ...
    Unpacking lzop (1.04-2build3) ...
    Setting up lzop (1.04-2build3) ...
    Processing triggers for man-db (2.12.0-4build2) ...
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lzop -d g.lzo
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: lzip compressed data, version: 1
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.lz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ lunzip g.lz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: XZ compressed data, checksum CRC64
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ mv g g.xz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ xz -d g.xz
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ file g
    g: ASCII text
    suryansh@LAPTOP-P5CN4E7M:/mnt/c/Users/LENOVO/Downloads$ cat g
    7069636f4354467b66316c656e406d335f6d406e3170756c407431306e5f
    6630725f3062326375723137795f37396230316332367d0a


on decoding by chat gpt
![image](https://github.com/user-attachments/assets/c5bd03fb-0a73-4c8c-a35c-1daf579975bb)

