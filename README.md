# Install-JDK-and-Setup-JAVA_HOME-on-Mac
Step by step process on how to install jdk and setup java_home on macOs

For MacOs having Apple Silicon chip...

Step 1: Open terminal (command+space) and type "java -version" in it.
        It will tell if there is any pre-existing version available in the system or not.
        
Step 2: If Java not present, open any browser (Chrome, Firefox, Safari) and go to https://www.oracle.com/java/technologies/downloads/

Step 3: Find the suitable version of Java according to you, and download the ".dmg" file from "Arm 64 DMG Installer" .

Step 4: After it has been installed, open the file and install it.

Step 5: Now, JDK is installed on your system.
        To check, open terminal (command+space) and type "java -version" and you will be able to see your respective jdk.


**To setup path for JAVA_HOME...**


Step 6: First check whether you have /zsh file or /bash file...
        To check, open terminal and type "echo $SHELL"
        
Step 7: SPECIFICALLY FOR /zsh shell...
        Check if the system contains /.zshenv file...to check type "ls -al" in terminal
        
Step 8: If not present, type "touch ~/.zshenv" in terminal.

Step 9: If already present, skip step 8 and type "/usr/libexec/java_home" and copy the java_home path.

Step 10: Now type "echo $JAVA_HOME" and check whether the java_home has been set or not.

Step 11: If not set, type "open ~/.zshenv" in terminal. It will open the /.zshenv file.

Step 12: Type "export $JAVA_HOME=path that you copied from step 9" and save it and close.

Step 13: Now type "source ~/.zshenv" to save the changes.

Step 14: To check whether the java_home has been set correctly or not, type "echo $JAVA_HOME" in the terminal.


Your JDK and Java_Home has been set correctly in the system.
