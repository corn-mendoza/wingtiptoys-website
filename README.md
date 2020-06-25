# Wingtip Toys Store Website

## Overview
Demo .NET Core Wingtip Toys Web Store website designed using Steeltoe Cloud Native libraries as part of the Wingtip Toys Services demos. This package includes an example of loading local nuget packages as part of a Docker build. 

## Requirements
This project utilizes different cloud native services along with a SQL Server approach to managing session data to support multiple instances running concurrently. A connection string to a SQL Server database is required for the application to function properly.

# Deploying the Web Store

This application is designed to load secrets from an optional file located in **secrets/appsettings.secrets.json**. All platforms can leverage this to inject sensitive SQL Server or service connection string information for the application or continue to use the appsettings.json file.

Sample **appsettings.secrets.json**

    {
        "ConnectionStrings": {
            "DefaultConnection": "<yourconnectionstring>"
        }    
    }  

