# 202334522_-_lecture_note_4.
Kernel:Core of OS that controls and communicates with hardware resource.
Shell: interface that allows users to communicate with kernel. Users runs applications and give commands through shell

## Shell commands
1.pwd: shows the currents path in a hierarchical directory
2.cd: change directory
3.ls: list files and directories
 - options: I show detailed information(long format)
 - Ih same as above,but size in units
4.More on ls
 -ls: List the files in the working directory
 -ls/bin: List the files in the /bin directory (or ant other directory we care to specify) 
 -ls -1: List the files in the working directory in long format
 -ls -1/etc/bin: List the files in the /bin directory and the /etc directory in long format
 -ls -la ..: List all files (even ones with names beginning with a period character,which are normally hidden) in the parent of the working directory in long format

## Manipulation
1.cp: copy files and directories
   -cp file1 file2: Copies the contents of file1 into file2. If file2 does not exist, It is created; otherwise, file2 is silently overwritten with the contents of file1.
   -cp -i file1 fil2: Like above however, since the "-i" option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
   -cp fil1 dir1: Copy the contents of file1 (into a file named file1) inside of directory dir1.
   -cp -R dir1 dir2: Copy the contents of directory dir1. If directory dir2 does not exist, It is created. Otherwise, it creates a directory names dir1 within directory dir2.
2.mv: move files and directories or rename them
   -mv file1 file2: If file2 does not exist, then file1 is renamed file2. If file2 exists, its contents are silently replaced with the contents of file1.
   -mv -i file file2: Like above however,since the "-i" option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
   -mv file1 file2 dir1: The file1 and file2 are moved to directory dir1. If dir1 does not exist, mv will exit with an error.
   -mv dir1 dir2: If dir2 does not exist, then dir1 is renamed dir2. if dir2 exists, the directory dir1 is moved within directory dir2.
3.rm: delete files and directories permantely and irreversevely
   -rm file1 fil2: Delete file1 and file2.
   -rm -i file1 file2: Like above however, since the "-i" option is specified, the user is prompted before each file is deleted.
   -rm -r dir1 dir2: Directories dir1 and dir2 are deleted along with all of their contents
4.mkdir: make a new directory
