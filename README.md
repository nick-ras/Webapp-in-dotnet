# .NET Web Application

This is a web application built using ASP.NET Core. It includes a clean and modular structure with areas for Identity, Controllers, Views, Models, and Data. The app is designed for easy configuration with environment variables and integrates well with Azure for cloud deployment.

## Table of Contents
- [Project Setup](#project-setup)
- [Prerequisites](#prerequisites)
- [Directory Structure](#directory-structure)
- [Running the Application](#running-the-application)
- [Environment Variables](#environment-variables)
- [Azure Deployment](#azure-deployment)
- [Testing](#testing)

## Project Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo/webapp-dotnet.git
   cd webapp-dotnet
   
Dependencies: Ensure you have .NET SDK installed and run:

```bash
dotnet restore
```
Build the Project: To build the application, execute:
```
```bash
dotnet build
```
Prerequisites
.NET SDK (Version: 5.0 or higher)
Azure Account (for cloud deployment)
Visual Studio Code or any preferred IDE for .NET development

Directory Structure
```bash
├── .azure                    # Azure-related configurations
├── .vs                       # Visual Studio-related files
├── Areas
│   ├── Identity
│   │   └── Pages            # Identity-related pages
├── Controllers               # Controller classes for app functionality
├── Data                      # Data access layer
├── Models                    # Application models
├── Properties                # Project properties
├── Views                     # Views for the app (Razor pages)
├── wwwroot                   # Static files (CSS, JS, Images, etc.)
├── obj                       # Temporary build files
├── Program.cs                # Main entry point of the application
├── WebAppStartup.csproj      # Project file containing dependencies
├── WebAppStartup.sln         # Solution file
├── .gitignore                # Git ignore configuration
└── README.md                 # Project documentation
```
##Running the Application
Run the App Locally: To run the application locally, use the following command:

```bash
dotnet run
```
This will start the application on your local machine, typically accessible at http://localhost:5000.

Run with Debugging: You can debug the application using your IDE (e.g., Visual Studio or VS Code). Make sure the debugging configuration is set for .NET Core.

##Environment Variables
The application is configured to use environment variables for sensitive data and configuration settings. Ensure that the following environment variables are set:

APP_SETTINGS – The application configuration settings.
DATABASE_URL – The database connection string.
SECRET_KEY – The secret key used for cryptography.
These variables can be set in your system, or you can use an .env file in your root directory for local development.

##Azure Deployment
I deployed with Azure, but you can choose how to deploye yourself, if needed

##Testing
Unit and integration tests are organized in the project. To run the tests, use the following command:

```bash
dotnet test
```
This will execute all tests and display the results.
