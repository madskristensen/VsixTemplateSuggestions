# VSIX Project Template Suggestions

[![Build status](https://ci.appveyor.com/api/projects/status/q04ebk3mf9btvgxh?svg=true)](https://ci.appveyor.com/project/madskristensen/vsixtemplatesuggestions)

---------------------------------------

A suggestion to improve the Visual Studio Extensibility (VSIX) templates. The templates in the repo are samples of what the output of better project templates can look like.

## Goals

* Follows best practices by default
* Eliminate API versioning conflicts
* Reduce time to *Wow!*
* Reduce concept count

## Features

* 2 Templates
  * [VSIX Project (with AsyncPackage)](src/VsixProject/)
  * [Empty VSIX Project](src/EmptyVsixProject/)
* Uses `<PackageReference>`
* References meta package with entire VSSDK
* References Roslyn Analyzers for best practice adherence
* No dump of VSSDK binaries in the /bin folder
* Resource file (.resx) no longer needed
* No strong name signing
* CSS file rolled into the HTML file
* Default icon added to demonstrate correct size
* Verbose code comments removed
* Removed unneeded `<Dependencies>` section in .vsixmanifest

## VS modification wishlist

* Built in code generation for .vsixmanifest and .vsct files
  * Update *Package* and *AssemblyInfo* attributes with values
* Build support for no .resx files into *BuildTools*
  * Then remove the *Madskristensen.VSSDK.Resourcer* NuGet package
* Support Project Overview page 
  * Then remove the *Index.html* file

## License
[Apache 2.0](LICENSE)