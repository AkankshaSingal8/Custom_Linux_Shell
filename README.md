# Custom_Linux_Shell
Designed and implemented a custom Unix shell using standard C libraries for internal and external commands like ‘cd’, ‘echo’, ‘pwd’, ‘ls’, ‘cat’, ‘date’, ‘rm’ and ‘mkdir’

Assumption for thread
&t is given at the end of the command after space
example: ls &t

EXIT  
exit command to exit the shell  
  
CD  
options to be added just after cd  
cd filename = current working directory is changed to filename  
cd filename -L = current working directory is changed to filename from environment  
cd filename -P = current working directory is changed to filename  
cd .. = current working directory is the parent  
cd / = current working directory is / or Home  


PWD  
options to be added just after pwd  
pwd = prints the current working directory  
pwd -L = prints the current working directory from environment  
pwd -P = prints the current working directory  
  
ECHO  
options to be added just after echo  
echo = prints whatever is given after echo  
echo -n = prints whatever is given after echo but removes the trailing  
echo -E = prints whatever is given after echo and does not interpret the backslashed  
  
LS  
options to be added at the end  
ls = list all the files excluding . and ..  
ls -a = list all files including . and ..  
ls -1 = list all files excluding . and .. in a single line  
  
DATE  
options to be added at the end  
date = prints the local date and time  
date -u = prints the UTC date and time  
date -R = output date and time in RFC 5322 format  
  
RM  
options to be added at the end  
checks if filename is given  
gives error if it is a directory  
rm filename = deletes file  
rm filename -v = gives message if deleted or if not able to delete  
rm filename -i = prompts if user wants to delete file  
  
MKDIR  
options to be added at the end  
checks if filename is given  
gives error if directory already exists  
mkdir filename = creates directory  
mkdir filename -v = gives message if created or if not able to create  
mkdir filename -m mode =  creates directory with given mode  
  
CAT  
options to be added at the end  
checks if filename is given  
gives error if file does not exist  
cat filename = prints the data in file  
cat filename -n = prints the line number  
cat filename -E = print $ sign at the end of each line  
  
