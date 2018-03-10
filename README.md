# setup gradle with binary zip folder in  linux 

1.install the gradle in your computer 
2.set environmental varibale to gradle  in windows
# Set environment Variable in windows
environmental Variable-Set Variabel of gradle of path  

# Set environment Variable in linux
download the binary of gradle and go through the command in terminal 

`$ mkdir /opt/gradle`
`$ unzip -d /opt/gradle gradle-4.6-bin.zip`
`$ export PATH=$PATH:/opt/gradle/gradle-4.6/bin`

# version of gradle in termial 
`$ gradle -v`

# and create a project folder
`mkdir project-Name`
`cd project-Name`

# Setup gradle project in your folder
`*gradle init*`  -create a src folder in project


# Define a task in build.gradle 

task copy(type: Copy, group: "Custom", description: "Copies sources to the dest directory") {
    from "src"
    into "dest"
} 

# Run that task by task name  
` ./gradlew <task Name>`  

# Define plugin in gradle

#only buildscript and other plugin script block are allowed before plugins ,no other statment are allowed

plugin{
    id="your plugin"
}  

# Overall to run the task in gradle 
`./gradlew tasks`

#The properties command tells you about a project’s attributes.
`./gradlew properties`

