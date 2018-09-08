# VSIX Project Template Suggestions

[![Build status](https://ci.appveyor.com/api/projects/status/ox04djmajibm3qqv?svg=true)](https://ci.appveyor.com/project/madskristensen/imagesprites)

---------------------------------------

My suggestion to what the Visual Studio Extensibility (VSIX) templates should look like.

## Goals

* Follows best practices by default
* Eliminate API versioning conflicts
* Reduce time to *Wow!*
* Reduce concept count


## Features

* 2 Templates
  * VSIX Project (with AsyncPackage)
  * Empty VSIX Project
* Uses `<PackageReference>`
* References meta package with entire VSSDK
* References Roslyn Analyzers for best practice adherence
* No dump of VSSDK binaries in the /bin folder
* Resource file (.resx) no longer needed
* No strong name signing
* CSS file rolled into the HTML file
* Default icon added to demonstrate correct size
* Verbose code comments removed
* Removed unneeded `<Dependencies>` section in .vsixmanife

## License
[Apache 2.0](LICENSE)