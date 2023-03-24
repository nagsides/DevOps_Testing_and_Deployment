# DevOps_Testing_and_Deployment
DevOps Testing and Deployment

## This repository follows the tutorial and code from
https://learn.microsoft.com/en-gb/dotnet/core/testing/unit-testing-with-dotnet-test

Also look at the oode available at:

https://github.com/dotnet/samples/tree/main/core/getting-started/unit-testing-using-dotnet-test

Initial commands for creating this app:

dotnet new sln -o unit-testing-using-dotnet-test
cd unit-testing-using-dotnet-test
dotnet new classlib -o PrimeService
cd PrimeService
mv Class1.cs PrimeService.cs
cd ..
dotnet sln add ./PrimeService/PrimeService.csproj
dotnet new xunit -o PrimeService.Tests
dotnet add ./PrimeService.Tests/PrimeService.Tests.csproj reference ./PrimeService/PrimeService.csproj
dotnet sln add ./PrimeService.Tests/PrimeService.Tests.csproj


