showall
=======

Simple extension of 'which' that traverses your complete $PATH environment for matches

The which command only prints out the first match it finds for an executable.
Often, I end up in environments where several entries as added to my PATH variable. 
This is sometimes from initrc scripts for a particular group within a company.

The showall script is a very script which basically traverses the complete PATH enviroment looking for matches.

For example, 
  % echo $PATH
  /bin:/usr/local/bin:/home/siva/bin:/usr/local/bin:/usr/bin:/cygdrive/c/Windows/system32:/cygdrive/c/
ws/System32/Wbem:/cygdrive/c/Program Files/Microsoft SQL Server/90/Tools/binn:/cygdrive/c/Program Fi
ared/9.0/DLLShared:/cygdrive/c/Windows/System32/WindowsPowerShell/v1.0:/usr/lib/lapack:/net/pharos/e

  % which ls
  /bin/ls

  % showall al
  /bin/ls
  /usr/bin/ls
