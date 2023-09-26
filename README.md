# Samples
Pipeline 1: Python Flask Application

Python Virtual Environment: The pipeline creates a Python virtual environment (venv) to isolate dependencies, ensuring a clean and consistent environment for the Flask application.

Dependency Management: It installs Python dependencies listed in a 'requirements.txt' file using pip install -r requirements.txt.

Artifact Packaging: After building the Flask application, it archives the application into a ZIP file, making it ready for deployment or distribution.

Ubuntu-Latest Agent: This pipeline uses the 'ubuntu-latest' agent, suitable for Python applications running on Linux environments.

Pipeline 2: Node.js Application

Node.js Installation: The pipeline installs Node.js 16.x, providing the required runtime environment for Node.js applications.

NPM Dependencies: It uses npm install to fetch and install Node.js dependencies listed in the 'package.json' file.

Artifact Publishing: The project files are copied and published as a pipeline artifact named 'drop,' making it accessible for downstream stages or deployments.

Ubuntu-Latest Agent: This pipeline also uses the 'ubuntu-latest' agent, suitable for Node.js applications running on Linux environments.

Pipeline 3: Java Maven Application

Java and Maven: The pipeline expects a Java application managed by Apache Maven. It runs 'mvn clean package' to compile, test, and package the application.

Artifact Publication: The Maven build output, typically located in the 'target' directory, is published as a container artifact named 'maven-build,' allowing for further deployment or distribution.

Ubuntu-Latest Agent: This pipeline uses the 'ubuntu-latest' agent, which is suitable for Java applications and Maven builds.

Pipeline 4: Java Ant Application

Java and Ant: This pipeline is designed for Java applications built with Apache Ant. It runs 'ant build' (replace 'build' with your Ant target) to build the Java application.

Artifact Publication: The Ant build output, usually found in the 'build' directory, is published as a container artifact named 'ant-build,' making it accessible for downstream processes.

Ubuntu-Latest Agent: Similar to the previous pipelines, it uses the 'ubuntu-latest' agent for Java and Ant-based builds.

Pipeline 5: .NET Core Application

.NET Core Version: The pipeline allows you to specify the version of the .NET Core SDK using the dotnetVersion variable. It's set to '6.0.x' by default.

Build Configuration: The pipeline performs a 'dotnet build' and 'dotnet publish' for .NET Core applications, using the specified project file(s) and build configuration.

Artifact Generation: It generates binaries, optionally zipped, and publishes them as build artifacts. The path to the project file(s) is customizable using the applicationPath parameter.

Windows-Latest Agent: This pipeline uses the 'windows-latest' agent, suitable for .NET Core applications running on Windows environments.

Pipeline 6: ASP.NET Application

ASP.NET Solution: This pipeline is designed for ASP.NET applications managed within a Visual Studio solution file (.sln).

NuGet Package Installation: It installs NuGet packages required for the ASP.NET application using the 'NuGetToolInstaller' task.

MSBuild Build: The pipeline runs 'dotnet build' using MSBuild with specified build configuration and project file(s) defined in the solutionPath parameter.

Artifact Publishing: It publishes build artifacts generated during the ASP.NET build process using the 'PublishBuildArtifacts' task.

Windows-Latest Agent: This pipeline uses the 'windows-latest' agent, suitable for building and deploying ASP.NET applications on Windows platforms.
