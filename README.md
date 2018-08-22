# IHostedServiceAsAService

A small example of a generic host based .NET core app which can be run as a Windows Service.

## Building and creating a service

### Build and publish

dotnet publish --configuration Release

### Define the service

sc create MyFileService binPath= "E:\Projects\IHostedServiceAsAService\IHostedServiceAsAService\bin\Release\netcoreapp2.1\win7-x64\publish\IHostedServiceAsAService.exe"

### Start the service

sc start MyService

For further details see my blog post [Running a .NET Core Generic Host App as a Windows Service](https://www.stevejgordon.co.uk/running-net-core-generic-host-applications-as-a-windows-service)
