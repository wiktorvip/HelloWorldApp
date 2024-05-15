# HelloWorldApp

dotnet new sln -o HelloWorldApp
cd HelloWorldApp
dotnet new mvc -n HelloWorldApp.Web
dotnet sln HelloWorldApp.sln add HelloWorldApp.Web/HelloWorldApp.Web.csproj
dotnet restore

dotnet build --no-restore --configuration release
dotnet publish --no-build --configuration release
