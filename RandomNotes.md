# .NET Core
- Installing dotnet runtime on Ubuntu
  Easiest way to install the .NET Core SDK or runtime is to follow the [Microsoft Instructions](https://docs.microsoft.com/en-au/dotnet/core/install/linux-ubuntu)
  For brevity, there are the command lines
  ```
  wget https://packages.microsoft.com/config/ubuntu/20.10/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
  sudo dpkg -i packages-microsoft-prod.deb
  sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y aspnetcore-runtime-5.0
  ```
  To install the SDK instead of the run time, use ```dotnet-sdk-5.0``` instead on the last line above.
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
  The contents of the output folder can be copied to another machine and run using just the .NET Core runtime, even if you built/published on Windows and moved the dll's to a Linux box.

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
