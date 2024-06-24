# Extending the Random class

Welcome to the NewRandom Class!

## Table of Contents
- [Extending the Random class](#extending-the-random-class)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [App File Structure](#app-file-structure)
  - [Features](#features)
  - [Screenshots](#screenshots)
  - [Technologies Used](#technologies-used)
  - [Installation and Operation](#installation-and-operation)
    - [1. Install IDE and JDK](#1-install-ide-and-jdk)
    - [2. Run the Program](#2-run-the-program)
  - [Future Considerations](#future-considerations)
  
## Overview

This application presents the user with a menu of functions to choose for generating/testing a desired randomized output. Each function is part of the NewRandom class which extends java.util.Random.

## App File Structure
The following is a brief overview of the file structure

[./src/main/java/NewRandomTest.java](https://github.com/voyagerfan/Extending-the-Random-Class/blob/main/src/main/java/NewRandomTest.java) - Main entry point for the program

[./src/main/java/NewRandom.java](https://github.com/voyagerfan/Extending-the-Random-Class/blob/main/src/main/java/NewRandom.java) - All functions from the NewRandom class.

## Features

The program includes the following features:

* Maven architecture for simplified builds and dependency management.
* Multiple functions that extend that the Random class:
  * **nextInt**(int low, int high) - returns a random int between low and high (inclusive)
  * **nextIntDigit**(int digits) - returns a random digit between 10^(digit-1) and (10^digit)-1 (inclusive)
  * **nextChar**() - returns a random alphabetic char
  * **nextChar**(char low, char high) - returns a random alphabetic char between low and high inputs (inclusive)
  * **nextChar**(char from, int i) - returns a random alphabetic char between from-i and from+i (e.g. from='h', i= 2 -> random range is from f to j)
  * **nextSpecialChar**() returns a non-alphanumeric char (ascii 33-126)
* Simplified test UI displayed in the console.

## Screenshots
*NOTE* the testing class is set to iterate 20 times.

**nextInt**(int low, int high) 

![](./screenshots/nextInt().png)

**nextIntDigit**(int digits)

![](./screenshots/nextIntDigits().png)

**nextChar**() 

![](./screenshots/nextChar().png)

**nextChar**(char low, char high) 

![](./screenshots/nextCar(from-to).png) 

**nextChar**(char from, int i)

![](./screenshots/nextChar(char-to-i).png) 

**nextSpecialChar**()

![](./screenshots/nextSpecialChar().png) 

## Technologies Used

- **Programming Languages:** Java
- **Tools:** Eclipse

## Installation and Operation

*Prerequistes:* **Java Development kit**, **an IDE**, **Google Maps API Key**, **Openweathermaps API Key**  

### 1. Install IDE and JDK

1) To run this program, you will need to install an IDE (e.g. [Eclipse](https://www.eclipse.org/downloads/) or [IntelliJ](https://www.jetbrains.com/help/idea/installation-guide.html#toolbox)) and the [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/downloads/).

2) Once you have installed an IDE and JDK, you may clone the repo and open the project folder or create your own project and copy the java files from the [src/main/java](https://github.com/voyagerfan/Extending-the-Random-Class/tree/main/src/main/java) folder. 


### 2. Run the Program
* From your IDE, you may now run the program.

## Future Considerations
While this program provides some key features and highlights basic programming concepts, it is limited in terms of input handling and testing robustness. These limitations have prompted the consideration of the following improvements:

* Error Handling
  * Implement additional programatic restrictions on user input ranges with appropriate messaging to the user.
* Unit testing
  * Replace UI console testing with JUnit tests to ensure the functions perform as expected.
* CI pipelining
  * Consolidate the Junit testing using Github actions.
  * Integrate builds and tests before merging  to protect the main branch.









