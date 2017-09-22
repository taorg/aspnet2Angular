# ASPNET2ANGULAR
Hola este es un ejemplo creado con .NET Core 2.0 SDK
El nuevo SDK incluye generador para Angular y React

La secuencia para generar la aplicació es:

```
➜ dotnet new angular -o aspnet2Angular
 Processing post-creation actions...
Running 'dotnet restore' on aspnet2Angular/aspnet2Angular.csproj...
  Restoring packages for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular/aspnet2Angular.csproj...
  Restore completed in 33.24 ms for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular/aspnet2Angular.csproj.
  Generating MSBuild file /Users/taorg/Projects/aspnet2Angular/aspnet2Angular/obj/aspnet2Angular.csproj.nuget.g.props.
  Generating MSBuild file /Users/taorg/Projects/aspnet2Angular/aspnet2Angular/obj/aspnet2Angular.csproj.nuget.g.targets.
  Restore completed in 1.89 sec for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular/aspnet2Angular.csproj.


Restore succeeded.

Description:

-------------------------------------------------------------------
IMPORTANT: Before running this project on the command line,
           you must restore NPM packages by running "npm install"
-------------------------------------------------------------------

Manual instructions: Run "npm install"
```
---

```
➜  aspnet2Angular npm install
npm WARN read-shrinkwrap This version of npm is compatible with lockfileVersion@1, but npm-shrinkwrap.json was generated for lockfileVersion@0. I'll try to do my best with it!
npm WARN deprecated coa@1.0.3: Please upgrade to 1.0.4 for node 0.10, 0.12, or to 2.0+ for node 4+
npm WARN deprecated chalk@2.0.1: Please upgrade to Chalk 2.1.0 - template literals in this version (2.0.1) are quite buggy.

> fsevents@1.1.2 install /Users/taorg/Projects/aspnet2Angular/node_modules/fsevents
> node install

[fsevents] Success: "/Users/taorg/Projects/aspnet2Angular/node_modules/fsevents/lib/binding/Release/node-v48-darwin-x64/fse.node" already installed
Pass --update-binary to reinstall or --build-from-source to recompile
```

---


```
➜  aspnet2Angular npm install
npm WARN read-shrinkwrap This version of npm is compatible with lockfileVersion@1, but npm-shrinkwrap.json was generated for lockfileVersion@0. I'll try to do my best with it!
npm WARN deprecated coa@1.0.3: Please upgrade to 1.0.4 for node 0.10, 0.12, or to 2.0+ for node 4+
npm WARN deprecated chalk@2.0.1: Please upgrade to Chalk 2.1.0 - template literals in this version (2.0.1) are quite buggy.

> fsevents@1.1.2 install /Users/taorg/Projects/aspnet2Angular/node_modules/fsevents
> node install

[fsevents] Success: "/Users/taorg/Projects/aspnet2Angular/node_modules/fsevents/lib/binding/Release/node-v48-darwin-x64/fse.node" already installed
Pass --update-binary to reinstall or --build-from-source to recompile
added 806 packages in 123.15s

➜  aspnet2Angular dotnet restore
  Restoring packages for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular.csproj...
  Restore completed in 30.76 ms for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular.csproj.
  Generating MSBuild file /Users/taorg/Projects/aspnet2Angular/obj/aspnet2Angular.csproj.nuget.g.props.
  Restore completed in 1.79 sec for /Users/taorg/Projects/aspnet2Angular/aspnet2Angular.csproj.
  
➜  aspnet2Angular dotnet run
Hosting environment: Production
Content root path: /Users/taorg/Projects/aspnet2Angular
Now listening on: http://localhost:5000
Application started. Press Ctrl+C to shut down.
```



---


## El opciones del nuevo generador en la version 2.x


---
```
➜  Projects dotnet -h
.NET Command Line Tools (2.0.0)
Usage: dotnet [runtime-options] [path-to-application]
Usage: dotnet [sdk-options] [command] [arguments] [command-options]

path-to-application:
  The path to an application .dll file to execute.

SDK commands:
  new              Initialize .NET projects.
  restore          Restore dependencies specified in the .NET project.
  run              Compiles and immediately executes a .NET project.
  build            Builds a .NET project.
  publish          Publishes a .NET project for deployment (including the runtime).
  test             Runs unit tests using the test runner specified in the project.
  pack             Creates a NuGet package.
  migrate          Migrates a project.json based project to a msbuild based project.
  clean            Clean build output(s).
  sln              Modify solution (SLN) files.
  add              Add reference to the project.
  remove           Remove reference from the project.
  list             List reference in the project.
  nuget            Provides additional NuGet commands.
  msbuild          Runs Microsoft Build Engine (MSBuild).
  vstest           Runs Microsoft Test Execution Command Line Tool.

Common options:
  -v|--verbosity        Set the verbosity level of the command. Allowed values are q[uiet], m[inimal], n[ormal], d[etailed], and diag[nostic].
  -h|--help             Show help.

Run 'dotnet COMMAND --help' for more information on a command.

sdk-options:
  --version        Display .NET Core SDK version.
  --info           Display .NET Core information.
  -d|--diagnostics Enable diagnostic output.

runtime-options:
  --additionalprobingpath <path>    Path containing probing policy and assemblies to probe for.
  --fx-version <version>            Version of the installed Shared Framework to use to run the application.
  --roll-forward-on-no-candidate-fx Roll forward on no candidate shared framework is enabled.
  --additional-deps <path>          Path to additonal deps.json file.
```

