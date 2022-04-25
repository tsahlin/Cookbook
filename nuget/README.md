# Nuget

### Creating a Nuget package

 - Open a cmd window inside a project directory and run `nuget spec`
 - Open the generated `*.nuspec` file in a text editor
 - When done with the nuspec file, run `nuget pack <my file>.nuspec`

### Inspecting a Nuget package

 - Rename the `*.nupkg` file to `*.zip` and unzip the contents

### Using a local folder as a package source

 - Create an empty folder
 - Open a cmd window and run `nuget add <some package>.nupkg -source <folder path>`
 - The nuget command will setup the necessary directory structure
 - Add the folder as a Nuget source in Visual Studio
 - More info: [Local feeds](https://docs.microsoft.com/en-us/nuget/hosting-packages/local-feeds)
