# Mega Player Robots API

<p align="center">
  <img src="./_docs/assets/icon.png" alt="Mega Player Robots API" width="150" />
</p>

## Overview

This .NET Core API is designed to serve JSON formatted data about bosses from the Mega Player series. It is a backend service built with .NET Core 3.1 and various modern dependencies for data management and API response handling.

Developed with Entity Framework Core and other modern .NET technologies, this project aims to provide a robust API for accessing Mega Player robot data.

<p align="center">
  <img src="./_docs/assets/carbon.png" />
</p>

## API Endpoints

| Method | Endpoint              | Description                               |
| ------ | --------------------- | ----------------------------------------- |
| GET    | `/api/v1/robots`      | Returns a list of all robots              |
| GET    | `/api/v1/robots/{id}` | Returns details of a specific robot by ID |
| POST   | `/api/v1/robots`      | Endpoint to create a new robot entry      |

## Techniques Used

- **Entity Framework Core:** ORM for data management.
- **RESTful API Design:** Ensures clear and effective communication endpoints.
- **Dependency Injection:** Used throughout to promote loose coupling and enhanced testability.

## Dependencies

| Package                                 | Version | Link                                                                                  |
| --------------------------------------- | ------- | ------------------------------------------------------------------------------------- |
| Microsoft.EntityFrameworkCore           | 3.1.8   | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8)           |
| Microsoft.EntityFrameworkCore.Design    | 3.1.8   | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8)    |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8   | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| Newtonsoft.Json                         | 12.0.2  | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2)                        |

## :gear: Project Structure

```
src
+-- ?? Controllers      [Routes for endpoints]
+-- ?? Models           [Database models]
+-- ?? Services         [Business rules]
+-- ?? Middlewares      [Intermediate functions between the HTTP request and the final server response]
+-- ?? Database         [Structures related to the database]
¦   +-- ?? DTOs             [Input Models and View Models (Data Transfer Objects)]
¦   +-- ?? EntityFramework  [Files related to the ORM Entity Framework]
```
