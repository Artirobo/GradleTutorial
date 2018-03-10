# setup gradle with binary zip folder in  linux 

# install the gradle in your computer 
# set environmental varibale to gradle  in windows
environmental Variable-Set Variabel of gradle of path 

# set gradle in linux  
#download the binary of gradle 
#go through the command 
$ mkdir /opt/gradle
$ unzip -d /opt/gradle gradle-4.6-bin.zip
#set environment variable in linux
$ export PATH=$PATH:/opt/gradle/gradle-4.6/bin

#see version 
$ gradle -v

# and create a project folder
mkdir project-Name
cd project-Name

#Setup gradle project in your folder
gradle init

#create a src folder in project

#define a task in build.gradle 

#run that task by task name  with ./gradlew <task Name> in terminal 

#To define plugin in gradle you can use  this
# only buildscript{} and other plugin{} script block are allowed before plugins{} ,no other statment are allowed
plugin{
    id="your plugin"
} 

#overall to run the task in gradle 
./gradlew tasks

