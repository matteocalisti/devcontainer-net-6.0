# devcontainer-net-6.0

## steps to create empty project

* install _vscode_

* install _Remote - Containers_ extension

* initialize devcontainer with command _Remote-Containers: Add Development Container Configuration Files_

    * Choose C# -> .net 6.0 -> lts

* Reopen the workspace as a Container

    * vscode will start the setup of the devcontainer

* _dotnet new sln_ will create a new empty solution

* _dotnet new web --output example/_ will create a new project called _example.csproj_ inside the folder _./example_

* _dotnet sln add example/example.csproj_ will add the newly created project to the solution

* _dotnet run --project example/example.csproj_ will build and run the application

    * _dotnet dev-certs https --trust_ is necessary to trust the https dev certificate
