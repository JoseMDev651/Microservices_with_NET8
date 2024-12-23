# Microservices_with_NET8

1.- Prerequisites

VS Code
Docker Desktop (running kubernetes)
Acoount on Docker Hub
Postman

2.- Commands from Terminal
    dotnet new webapi -n PlatformService
    code -r PlatformService
    dotnet add package AutoMapper.Extensions.Microsoft.DependencyInjection
    dotnet add package  Microsoft.EntityFrameworkCore
    dotnet add package  Microsoft.EntityFrameworkCore.Design
    dotnet add package  Microsoft.EntityFrameworkCore.InMemory
    dotnet add package  Microsoft.EntityFrameworkCore.SqlServer
3.- Create Models
	Create forlder Models
	Create model file inside (in this Platform.cs)
4.- DbContext
	New folder (Data)
	New file inside (AppDbContext.cs)
	add AppDbContext to program.cs (builder.Services)
5.- Repository
	Add new file in Data folder -> IPlatformRepo (for dependency injection)
	Add new file PlatformRepo.cs
		
	
