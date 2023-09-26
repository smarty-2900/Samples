# Samples

# Pipeline Configurations

This repository includes pre-configured CI/CD pipelines for various types of applications and development stacks. Each pipeline is designed to automate the build and deployment process for a specific technology stack.

## Pipeline 1: Python Flask Application

- **Python Virtual Environment:** Creates a Python virtual environment (venv) for isolating dependencies.
- **Dependency Management:** Installs Python dependencies from 'requirements.txt'.
- **Artifact Packaging:** Archives the Flask application into a ZIP file.

## Pipeline 2: Node.js Application

- **Node.js Installation:** Installs Node.js 16.x for Node.js applications.
- **NPM Dependencies:** Installs Node.js dependencies from 'package.json'.
- **Artifact Publishing:** Copies and publishes project files as a 'drop' artifact.

## Pipeline 3: Java Maven Application

- **Java and Maven:** Expects a Java application managed by Apache Maven.
- **Build and Package:** Runs 'mvn clean package' to compile, test, and package the application.
- **Artifact Publication:** Publishes Maven build output as a 'maven-build' artifact.

## Pipeline 4: Java Ant Application

- **Java and Ant:** Designed for Java applications built with Apache Ant.
- **Build:** Runs 'ant build' (customize 'build' with your Ant target) to build the Java application.
- **Artifact Publication:** Publishes Ant build output as an 'ant-build' artifact.

## Pipeline 5: .NET Core Application

- **.NET Core Version:** Specify the .NET Core SDK version with the `dotnetVersion` variable.
- **Build Configuration:** Performs 'dotnet build' and 'dotnet publish' for .NET Core applications.
- **Artifact Generation:** Generates binaries and publishes them as build artifacts.

## Pipeline 6: ASP.NET Application

- **ASP.NET Solution:** Designed for ASP.NET applications within a Visual Studio solution (.sln).
- **NuGet Package Installation:** Installs required NuGet packages.
- **MSBuild Build:** Runs 'dotnet build' with specified configurations and project file(s).
- **Artifact Publishing:** Publishes build artifacts generated during the ASP.NET build process.


Feel free to explore each pipeline's configuration for more details on how they work.
