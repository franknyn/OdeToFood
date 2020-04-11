# OdeToFood


### ASP.NET Core 3

## Module 5 (Working with SQL Server and the Entity Framework Core)

### Clip 4 (Using the Entity Framework Tools)

Starting in 3.0, the dotnet ef command-line tool is no longer included in the .NET Core SDK. Before you can execute EF Core migration or scaffolding commands, you’ll have to install this package as either a global or local tool. To install the latest version as a global tool, use the following command:

```
dotnet tool install --global dotnet-ef

// Inside OdeToFood/OdeToFood.Data run
dotnet ef dbcontext info -s ../OdeToFood/OdeToFood.csproj
dotnet ef migrations add initialcreate -s ../OdeToFood/OdeToFood.csproj
dotnet ef database update -s ../OdeToFood/OdeToFood.csproj
```
