# Nuget

 - [Creating a Nuget package](#creating-a-nuget-package)
 - [Inspecting a Nuget package](#inspecting-a-nuget-package)
 - [Using a local folder as a package source](#using-a-local-folder-as-a-package-source)
 - [Overwriting an existing package version](#overwriting-an-existing-package-version)

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

### Overwriting an existing package version

 - Not possible - manually remove the version folder (`source/package-name/version`) and then use `nuget add` to re-add the package.
