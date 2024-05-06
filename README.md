# OS-LAB-2

1. Exercise_1 - Write a shell script program that prints shell scripting is fun.

   CODE:
        echo "Shell scripting is fun."
   
   img.src="<img width="1465" alt="shell scripting is fun" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/eb9b206e-fdac-4a51-8863-7fe9a424e0c8">


2. Exercise_2 - Write a shell script program that modifies the shell script from ques 1 to include the variable. the variable will holdthe content of the messahe "Shell Scripting is fun"


   CODE:
         message="Shell Script is nice"
         echo "$message"
   img.src="<img width="1470" alt="ShellScriptIsNice" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/674dc56c-d550-4ee1-87ad-22ccb4b9bfaa">

   
 

3. Exercise_3 - Store the output of the command “hostname” in a variable. Display “This script is running on _.” where “_” is the output of the “hostname” command.

    CODE: 
        hostname=$(hostname)
        echo "This script is running on $hostname."
   img.src="<img width="1463" alt="hotsname" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/ecfbb709-f9db-4830-b11e-88c4816f6ca7">




4. Exercise_4 - Write a shell script to check to see if the file “file_path” exists. If it does exist, display “file_path passwords are enabled.” Next, check to see if you can write to the file. If you can, display “You have permissions to edit “file_path.””If you cannot, display “You do NOT have permissions to edit “file_path””

    CODE:
         file_path="file1.txt"
echo "file1.txt"

if [ -f "$file1.txt" ]; then
    echo "$file_path does not  exists."

    else
echo "file found $file"

    fi

img.src="<img width="1372" alt="filepath" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/e53f28da-0773-4e0a-a175-0a9e09778f53">

    
    
5. Exercise_5 - Write a shell script that displays “man”,”bear”,”pig”,”dog”,”cat”,and “sheep” on the screen with each appearing on a separate line. Try to do this in as few lines as possible.
   
    CODE:
         ANIMALS="man bear pig dog cat sheep"
for ANIMAL in $ANIMALS
do
  echo $ANIMAL
done

    img.src="<img width="1464" alt="animals" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/28efaa05-3f16-4b8a-b92e-cce9c133ba9f">

6. Exercise_6 - write a shell script that prompts the user for a name of a file or directory and reports if it is a regular file, a directory, or another type of file. Also perform an ls command against the file or directory with the long listing option.

  CODE:
       read FILE
if [ -f "$ankita.txt" ]
  then
    echo "$ankita.txt is a reguler file"
elif [ -d "$ankita.txt ]
  then
    echo "$ankita.txt is a directory"
else
    echo "$ankita.txt is another type of file"
fi
ls -l $ankita.txt
else
    echo "File or Directory '$ankita.txt' does not exists."
fi

 img.src="<img width="1196" alt="fileORdirectory" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/827e9ed5-8705-4497-9c43-c55811a82679">




7. Exercise_7 - Modify the previous script to that it accepts the file or directory name as an argument instead of prompting the user to enter it.

CODE:
    FILE=$1
if [ -f “$ankita.txt” ]
  then
    echo “$ankita.txt is a reguler file”
elif [ -d “$ankita.txt” ]
  then
    echo “$ankita.txt is a directory”
else
   echo “$ankita.txt is another type of file”
fi
ls -l $ankita.txt

img.src="<img width="1064" alt="argumentprompt" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/7ea97bc1-0567-4f6b-9554-300c09d951e9">



 8. Exercise_8 - Modify the previous script to accept an unlimited number of files and directories as arguments.

 Code:
      FILES=$@
for FILE in $arithmatic.sh
  do
    if [ -f “$arithmatic.sh” ]
      then
         echo “$arithmatic.sh is a reguler file”
    elif [ -d “$arithmatic.sh” ]
      then
         echo “$arithmatic.sh is a directory”
    else
         echo “$arithmatic.sh is another type of file”
    fi
   ls -l $FILE
  done
~        

 img.src=<img width="1288" alt="unlimited" src="https://github.com/ankitaa19/OS-LAB-2/assets/142775992/44420b09-4903-41bb-9779-e58130796c98">


 





