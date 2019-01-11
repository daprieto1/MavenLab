# Maven Basic Concepts

In this laboratory we are going to talk about the most basic concepts of Maven. A lot of IDE's like IntelliJ, Netbeans or others have support for maven pluggins, but in this laboratory we must to use just the terminal in order to maintain our focus on Maven.

## Deliverable

At the end of this laboratory you have to deliver a respository in GitHub where you demostrate the execution for each step. Additionally, in the README file you have to present an inform where you respond to all the questions or tasks that appear during the laboratory.

## Install Maven

Follow the instructions at maven.apache.org/install.html to install Maven on Windows, MacOS, or Linux.

Or, you can choose from one of the options below.

**Para instalar en MacOS**

`brew install maven`

**Para instalar en Linux**

`sudo apt-get install maven`

## Create Maven Project

Creating Maven projects is based on the concept of an archetype. Think of an archetype as a predefined template, like a blueprint from which we can generate projects.

> **Task:** 
>
> * Create a new maven project using the command `mvn archetype:generate -B -DgroupId=edu.eci -DartifactId=file-spy`, take screenshots.
> * What do means the -B option in the command?
> * What do means the -D option in the command?
> * What do means the groupId, artifactId properties in the command?
> * Describe the content of the directory that has been created.
> * Create the folders `src/main/resources` and `src/test/resources`

## POM file 
POM stands for Project Object Model And this file represents a one stop configuration for the entire project. Open the file to answer the next questions.

> **Task:**
>
> * What do means the word SNAPSHOT in the version value?
> * What is the purpose of the packing tag into the POM file?
> * What is the purpose of the dependencies and dependency tags into the POM file?

## Dependency Management

A dependency is a Java library that this project depends on. While developing Java applications, you'll almost always be using other developers libraries, in addition to your own. So if you want to use code that isn't a part of the Java core library, you'll need to add that library as a dependency. Dependencies and Maven are declared inside this dependencies element. With each dependency represented by its own dependency element. Naming follows the GAV convention which stands for Group Artifact and Version.


