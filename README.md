# linux_reference
## Table of Contents
- [Secure shell ssh/login](#login)
- [Create a file or directory](#create-file)
- [Open a file and navigate/less](#less)
- [Remove a file/directory](#remove-file)
- [Secure copy/scp](#scp)

## login
ssh -p <port_number> user@<server_name or ip_address>
### For Endeavour server
```ssh -p 15551 endeavour5@endeavourtech.ddns.net```

user id : endeavourn </br>
password: <Idiot_this_is_a_secret>

## Create File
touch <file_name> </br>
vi <file_name> </br>
**:q** to quit without saving </br>
**:q!** to force quit wihtout saving the changes </br>
**:wq** to save and quit </br>
To create a directory: </br>
mkdir

## Remove file
rm <file_name> </br>
To remove a directory: </br>
rm -r <name>

## less
less <file_name_which_you_want_to_read> </br>
If you want to put in "follow" mode.(Usually log file auto loads when new data comes) </br>
less +F <file_name> </br>

**Spacebar**: Move forward one page. </br>
**b**: Move back one page. </br>
**q**: Quit less. </br>
**/search_term**: Search forward for a specific term. </br>
**n**: Move to the next occurrence of the search term. </br>
**k**: Scroll up one line. </br>
**j**: Scroll down one line. </br>
**g**: Go to the beginning of the file. </br>
**G**: Go to the end of the file. </br>


## scp
### Moving from server to local:
```scp -3 scp://endeavour@endeavourtech.ddns.net:15551/~/linux-sept2024/sample3/sample.pdf Downloads/```

### If you are using default port 22:
```scp endeavour@endeavourtech.ddns.net:~/linux-sept2024/sample3/sample.pdf ~/linux-sept2024/sample3/```
