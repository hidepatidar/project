---
description: >-
  file compressing is a data compression method we use compressing becuase it is
  easy to transfer and more reason
---

# File compressing

### **BzipZ and Bunzip2**

```
# bzip2 filename

# bzip2 file1 file 2 file3

# bzip2 /root/d1/*

# bzip2 /root/d1/*.txt

# bzip2 *.log

#bzip2 s*

# bzip2 *

# bunzip2 /root/d1/ip*

# bunzip2 filename.bz2

# bunzip2 messeges1.bz2 messegess2.bz2

# bunzip2 messeges*

# bunzip2 *.log.bz2

# bunzip2 s*

# bunzip2 *
```

### **Gzip and Gunzip**

```
# gzip filename 

#gzip messeges2

# gzip messeges3 messeges4

# gzip *.log

# gzip s*

# gzip *

# gunzip filename.gz

# gunzip messeges.gz

# gunzip mese2.gz log.gz

# gzip *.log.gz

# gzip file1 fiule2 file3

# gunzip *

# gzip -r log/

# gunzip -r log/

# gzip /root/d1/*

# gunzip /root/d1/*

# gzip /root/ip*

# gunzip /root/ip*

# gzip -r /root/d1/

# gunzip -r /root/d1
```

### **zip and unzip**

```
# zip messege.zip messages3

# zip mese.all.zip messeg1 mese2 mese4

# zip log.zip *.log

# zip all-file.zip *

# zip -r log.zip log

# zip filename.zip filename

# unzip messe.zip

# zipinfo messe-all.zip

# unzip messe-all.zip

# unzip messe-all.zip -d mes

# unzip filename.zip

# zip filename.zip

# zip -r log.zip log/

#unzip log.zi
```

### **7z**

```
 # yum install epel-release.noarch     -   installation in rpm based linux
         
# yum install p7zip
         
# 7za --help
         
# 7za a messe.7z messe
         
# 7z a messe.7z messe
         
# 7za e messe.7z messe
         
# 7za a log.7z log/
         
# 7za e log.7z -o log
         
# 7za -r a log.7z log/
         
# 7za e -olog2 log.7z
         
# 7z e mess.7z
         
# 7zz a log.7z log
         
# 7z x log.7z
         
# 7z e log.7z
         
# 7z l mess.7z
         
# 7z t mess.7z
         
# 7z a d1.7z -r /root/d1/
         
# 7z | d1.7z
         
# 7z e d1.7z
```

### **tar and untar**

```
# tar -cvf messages.tar messages3
         
# tar -cvf messages-file.tar messages messages4 messages5
         
# tar -xvf messages-file.tar
         
# tar -cvf log.tar log/
         
# tar - xvf log.tar
         
# tar -cvf filename.tar directory
         
# tar -cvf filename.tar die1 dir2 dir3
         
# tar -xvf filename.tar
         
# tar -xvf d1.tar
         
# tar -cvf messages.tar messeges
         
# tar -cvf ip.tar ip*
         
# gzip file.tar
         
# tar -xvf d1.tar.gz
         
# gunzip file.tar
         
# bzip2 d1.tar
         
# bunzip2 d1.tar.bz2
         
# tar -cjvf log.bz2 log/
         
# tar -czvf log.tgz log/
         
# tar -cjvf filename.tgz file
         
# tar -xjvf filename.tbz
         
#  tar -czvf filename.tgz file
         
# tar -xzvf filename.tgz
```

###
