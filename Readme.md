## Fsharp + Paket + SQLProvider Woes

```powershell
dotnet new sln -n TestMe
dotnet new console -lang 'F#' -o SqlTP
dotnet sln add .\SqlTP\SqlTP.fsproj
dotnet new tool-manifest
dotnet tool install paket
dotnet tool restore
dotnet paket init
dotnet paket add SQLProvider --version 1.1.101 --interactive # add Y to add dependency
```
