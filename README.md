# neofetch_auto_execute
Guide to executing neofetch everytime you open a bash terminal

Step 1: Check if you have neofetch:

  $ neofetch
  

Step 2: If neofetch is not installed, install it:

  $ sudo apt install neofetch
  

Step 3: Create startup.sh file:

  cd to directory you would like to create the file
  
    $ cd /home/john/Projects/ (/home/john/Projects/ is the directory I used. Replace this with the directory you want to use.)
    
  create shell script file
  
    $ touch startup.sh
    

Step 4: Edit startup.sh file, adding shebang line and neofetch execution:

  $ nano startup.sh
  
    #!/bin/bash
    neofetch
    

step 5: Add execution permissions to startup.sh file:

  $ chmod +x startup.sh
  

step 6: Add line to .bashrc file

  $ echo "/home/john/Projects/startup.sh" >> ~/.bashrc (/home/john/Projects/ is the directory I used. Replace this with the directory you want to use.)
  

Step 7: Open a bash terminal to ensure it is working correctly
