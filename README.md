# sts_security_soc
this repo for a project using Splunk to get logs from Linux server this check attracts 

#first for download Splunk in Linux `wget` this tool ` wget -O splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz "https://download.splunk.com/products/splunk/releases/9.2.0.1/linux/splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz" `

* The ###`wget` command is a utility for downloading files from the internet using various protocols such as HTTP, HTTPS, and FTP.
# Installation process
* inter root access by `sudo su root`
* access for  directory  `cd  /opt  ` create splunk dir : `mkdir splunk`  `cd splunk` 
*  ` wget -O splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz "https://download.splunk.com/products/splunk/releases/9.2.0.1/linux/splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz" `
* ls check in the file is installed
** ---for Handel file download ---(tar)
     tar: The command-line utility for manipulating tar archives.
     -xzv: Options for the tar command:
     -x: Extract the contents of the archive.
     -z: Use gzip to decompress the archive.
     -v: Verbose mode, which displays detailed information about the extraction process.
     -C /opt: Change to the /opt directory before extracting files.
     -f filename: Specifies the input file (archive) to be extracted. In this case, file name is the 
**
* tar -xzvC /opt -f splunk-9.2.0.1-d8ae995bf219-Linux-x86_64.tgz
* start config  Splunk `cd bin` 
* we can search for  suplunk file by `ls |grep splunk` will make list
* to start config `./splunk status`
* after add admin password & username +password for user access
* just start `./splunk start`
* or jsut /opt/suplunk/bin/suplunk start --accept-license

