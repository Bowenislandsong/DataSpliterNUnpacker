# DataSpliterNUnpacker
This project is capable of splitting a dataset into different zip files and/or unpack all zip files in a folder

# Dependency 
- commons-io-2.6.jar
- zip4j_1.3.2.jar
- java 1.8

# Spliter Environment & Running Instruction 

Place the files in a sibling folder as Resource and Coding.

Run with "java -cp "zip4j_1.3.2.jar:commons-io-2.6.jar:" Main  <Resource_folder> <Code_Folder> <#ofNodes>"

For example: "java -cp "zip4j_1.3.2.jar:commons-io-2.6.jar:" Main Resource Code 5"

## Jar

Using Packed jar File: "java -jar java -jar Unpacker.jar <Resource_folder> <Code_Folder> <#ofNodes>"

For Example: "java -jar Unpacker.jar Resource Code 5"

# Unpacker Environment & Running Instruction

Place the files in a sibling folder as Target unpacking folder.

Run with "java -cp "zip4j_1.3.2.jar:commons-io-2.6.jar:" Main  <Target Folder>"

For example: "java -cp "zip4j_1.3.2.jar:commons-io-2.6.jar:" Main Target_Folder"

## Jar

Using Packed jar File: "java -jar java -jar Unpacker.jar <Target Folder>"

For Example: "java -jar Unpacker.jar Target_Folder"

## Output

Application will return on "System.exit" an int value for the actual number of nodes needed. This number will be equal or less than claimed number of nodes.

Output of the application will be zip files named "Distribute#". # will be based 0 to number of nodes required-1. THe zip file contains code and segmented recourses.
