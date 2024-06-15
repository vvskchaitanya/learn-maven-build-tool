# Learn Maven Build Tool

This project is a simple Maven-based Java application designed to help understand Maven's build lifecycle, phases, and commands.

## Prerequisites

- Java Development Kit (JDK) installed
- Apache Maven installed

## Installing Apache Maven

Follow these steps to install Apache Maven on your system:

### 1. Download Maven

Go to the [official Apache Maven website](https://maven.apache.org/download.cgi) and download the latest version of Maven. Choose the binary zip archive format.

### 2. Extract the Maven Archive

Once the download is complete, extract the contents of the Maven archive to a directory on your computer. For example, on Unix-based systems, you can use the following command in the terminal:

### 3.To verify Maven installation, run:

```sh
mvn -version
```

## Getting Started

### Generate New Maven Project:

To generate a new Maven project, open a terminal or command prompt window and run the following command:

```sh
   mvn archetype:generate -DgroupId=com.example -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

### Explore the Project:
- Once the project generation is complete, navigate to the project directory. 
- You can now explore the generated Maven project and start working on Java application.
- View and modify the source code, dependencies, and project configuration as needed.
- Use Maven commands to compile the source code, run tests, package the application, and perform other build tasks as required.

### Maven Lifecycle Phases

- **validate:** Validate the project is correct and all necessary information is available.
- **compile:** Compile the source code of the project.
- **test:** Test the compiled source code using a suitable unit testing framework.
- **package:** Take the compiled code and package it in its distributable format, such as a JAR or WAR.
- **verify:** Run any checks to verify the package is valid and meets quality criteria.
- **install:** Install the package into the local repository for use as a dependency in other projects locally.
- **deploy:** Copy the final package to the remote repository for sharing with other developers and projects.

### Customizing the `pom.xml`

To add more dependencies, edit the `<dependencies>` section in the `pom.xml` file. For example:

```
<dependencies>
    <dependency>
        <groupId>org.apache.commons</groupId>
        <artifactId>commons-lang3</artifactId>
        <version>3.12.0</version>
    </dependency>
</dependencies>
```

### Basic Commands

1. **Clean the project:**
```sh
mvn clean
```
2. **Compile the source code:**
```sh
mvn compile
```
3. **Run unit tests:**
```sh
mvn test
```
4. **Package the compiled code:**
```sh
mvn package
```
5. **Install the package locally:**
```sh
mvn install
```
6. **Deploy the package to a remote repository:**
```sh
mvn deploy
