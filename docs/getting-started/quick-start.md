Install the nexus-tool:
```powershell
dotnet tool install --global nexus-tool
```

From an empty directory run:
```powershell
nexus init -n "HelloWorld"
```

Add your own service (optional):
```powershell
nexus add-service -n "people"
```
A detailed guide on how to add new services can be found here

Run the supporting services:
```powershell
nexus run local
```

Develop/Run services from the IDE as necessary
