# .NET Core
- Building and Run a project
  ```
  dotnet restore
  dotnet run --project [your-project-name] 
  ```
  - Note depending on your launchSettings.json, yoru project may default to ```localhost:50000```. You can override that with the ```--url``` option (note 0.0.0.0 if you want remotely connect to 
  ```
  dotnet run --project [your-project-name] --url=https://localhost:5003
  ```

- Publish a project
```
dotnet publish -c Release -o out
```

- Run the published app
```
dotnet out/[your-project-name].dll
```


# Setting up a Windows Dev Box/Laptop
- Software
  - WSL
  - Docker
  - Visual Studio
  - Visual Studio Code
  
  
  
# Non-store Updates for MSIX apps
https://docs.microsoft.com/en-us/windows/msix/non-store-developer-updates
