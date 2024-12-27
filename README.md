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
5.- Repository (Data folder)
	Add new file in Data folder -> IPlatformRepo (for dependency injection)
	Add new file PlatformRepo.cs -> Implementation Interface IPlatformRepo functions

6.- Services(Program.cs)
	AddDBContext (In this example InMem but you can change to SQLServer). For development environments is more quick In Mem.
	Add.Scopped
7.- Terminal
	dotnet build
8.- Repository (Data forlder)
	Add file PrepDb.cs.
	Note: Add in Program.cs PrepDb.PrepPopulation(app);
	Terminal: dotnet build
		  dotnet run
9.- DTOs
	Create a new folder Dtos
	Create a new file inside Dtos -> PlatformReadDto.cs
	Create a new file inside Dtos -> PlatformCrateDto.cs
10.- Automapper
	PlatformService.csproj (<PackageReference Include="AutoMapper.Extensions.Microsoft.DependencyInjection" Version="12.0.1" />)
	Registry automapper for dependency injection
		Program.cs: builder.Services.AddAutoMapper(AppDomain.CurrentDomain.GetAssemblies());
	New folder Profiles
	New file PlatformsProfile.cs
	

	
 
	
		
	
