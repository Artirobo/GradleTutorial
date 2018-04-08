# Setup gradle with binary zip folder in  Linux 

1. Install the gradle in your computer 
2. Set environmental variable to gradle in Windows

# Set environment Variable in Windows
- Set Variable of gradle of path  

# Set environment Variable in Linux
Download the binary of gradle and go through the command in terminal 

- `$ mkdir /opt/gradle`
- `$ unzip -d /opt/gradle gradle-4.6-bin.zip`
- `$ export PATH=$PATH:/opt/gradle/gradle-4.6/bin`

### Version of gradle in termial 
- `$ gradle -v`

# Create a project folder
- `mkdir project-Name`
- `cd project-Name`

# Setup gradle project in your folder
- `*gradle init*`  
- Create a src folder in project

# Define a task in build.gradle 
```
task copy(type: Copy, group: "Custom", description: "Copies sources to the dest directory") {
    from "src"
    into "dest"
} 
```

# Run that task by task name  
- ` ./gradlew <task Name>`  

# Define plugin in gradle

- Only buildscript and other plugin script block are allowed before plugins ,no other statment are allowed
```
plugin{
    id="your plugin"
}  
```
### Overall to run the task in gradle 
`./gradlew tasks`

### The properties command tells you about a project’s attributes.
`./gradlew properties`

