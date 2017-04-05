This branch builds MSBuilds for our portable toolsets.
Call cibuild-jet.cmd to build automatically (better git-clean before that). Should have VS 14 installed in the default location.
Special settings: a separate build config which builds x64 and full framework and has #defines set up so that it were mono/*nix friendly as well.
The stuff from bin\Release-Jet\Windows_NT_Deployment is then planted into repo ssh://git-hosting.labs.intellij.net/dotnet-libs.git branch master folder Toolset\MSBuild\Lib, see readme there for further instructions.