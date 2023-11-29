#QEats :- food ordering app

## Overview
QEats is a popular food ordering app that allows users to browse and order their favourite dishes from nearby restaurants.
During the course of this project,
Built different parts of the QEats backend which is a Spring Boot application.
Several REST API endpoints are implemented to query restaurant information and order food.
It improved the app performance under large load scenarios as well as included an advanced search feature in the app.

![image](https://github.com/SoumyaMehta/QEats/assets/69056406/8ca557bf-f8d6-4051-8694-1ac973fe0c7b)

![image](https://github.com/SoumyaMehta/QEats/assets/69056406/5061db46-abba-48fb-a98c-8ab8b2ae7080)

![image](https://github.com/SoumyaMehta/QEats/assets/69056406/4690177a-7eb7-4d2f-80f6-3d1a2cdd51c0)

# Pre-requisites

* Java 1.8/1.11/1.15
* Gradle 6

# How to run the code

We have provided scripts to execute the code.

Use `run.sh` if you are Linux/Unix/macOS Operating systems and `run.bat` if you are on Windows.

Internally both the scripts run the following commands

* `gradle clean build -x test --no-daemon` - This will create a jar file `geektrust.jar` in the `build/libs` folder.
* `java -jar build/libs/geektrust.jar sample_input/input1.txt` - This will execute the jar file passing in the sample input file as the command line argument

 Use the build.gradle file provided along with this project. Please change the main class entry under the `jar` task

```
 manifest {
        attributes 'Main-Class' : 'com.geektrust.backend.App' //Change this to the main class of your program which will be executed
    }
```

in the build.gradle if your main class has changed.

# How to execute the unit tests

 `gradle clean test --no-daemon` will execute the unit test cases.

# Help

You can refer our help documents [here](https://help.geektrust.in)
You can read build instructions [here](https://github.com/geektrust/coding-problem-artefacts/tree/master/Java)