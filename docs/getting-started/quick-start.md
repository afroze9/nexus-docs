Install the nexus-tool:
```powershell
dotnet tool install --global nexus-tool
```

From an empty directory run:
```powershell
nexus init "hello-world"
```

Add your own service (optional):
```powershell
nexus add service "new-service"
```
A detailed guide on how to add new services can be found [here](./new-service.md)

Run the supporting services:
```powershell
nexus run local
```

Develop/Run services from the IDE as necessary
