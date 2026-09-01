# Test-Taste Console Application

This is a .NET console application that retrieves data from the `le-systeme-solaire` API and outputs information about planets, their moons, average moon gravity, and average moon temperature to the console.

## Prerequisites

- .NET 5.0 SDK (or compatible .NET environment)
- Active internet connection

## Configuration (API Key)

The application accesses data from the `le-systeme-solaire` API. To ensure smooth operation and avoid rate limiting, an API key must be specified in the `App.config` file located inside the `Test-Taste-Console-Application` directory.

### Setting up the `App.config`

1. Navigate to the `Test-Taste-Console-Application` folder.
2. Open the `App.config` file. If it doesn't exist, create it with the content shown below.
3. Replace the `value` attribute for the `ApiKey` key with your valid API token.

Example `App.config`:
```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <appSettings>
    <add key="ApiKey" value="add-api-key" />
  </appSettings>
</configuration>
```

## Running the Application

To run the application, open your terminal, navigate to the `Test-Taste-Console-Application` directory where the `.csproj` file is located, and execute the following command:

```bash
dotnet run
```

This will automatically build and execute the application. 

### Expected Output
The application outputs the following tabular data to the console sequentially:
1. Planets and their Average Moon Gravity
2. Moons and their Mass
3. Planets, their Semi-Major Axis, and Total Number of Moons
4. Planets and their Average Moon Temperature
