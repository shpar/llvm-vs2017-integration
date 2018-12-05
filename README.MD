# LLVM Visual Studio 2017 Integration

## Update 5.12.2018

This is a simple update to arves100's original repo which sets up LLVM integration in Visual Studio 17 (MSBuild 15.9) for LLVM 8.0.0. Just follow the instructions below and note that you might have to create a symlink cl.exe to the appropriate cland executable in your LLVM installation folder for this to work.

### Automatic Installation

Open a command prompt with Administrator rights (DO NOT OPEN AutoSetup.bat with admin rights it won't load the files)

Go to the folder where AutoSetup.bat exists and type "AutoSetup"

### Manual Installation (If Automatic dosen't work)

Go to "[Your Visual Studio Installation Directory]\Common7\IDE\VC\VCTargets\Platforms"

##### Performing x86 Toolset installation
- Go to Win32\PlatformToolset
- Create 2 folders called LLVM-vs2017 and LLVM-vs2017_xp
- Go to LLVM-vs2017
- Copy all files that starts with Toolset-llvm-vs2017-x86
- Rename the name of all this files (not the extensions) into Toolset
- Now go to LLVM-vs2017_xp
- Copy all files that starts with Toolset-llvm-vs2017-xp-x86
- Rename the name of all this files (not the extensions) into Toolset

##### Performing x64 Toolset installation
- Go to x64\PlatformToolset
- Create 2 folders called LLVM-vs2017 and LLVM-vs2017_xp
- Go to LLVM-vs2017
- Copy all files that starts with Toolset-llvm-vs2017-x64
- Rename the name of all this files (not the extensions) into Toolset
- Now go to LLVM-vs2017_xp
- Copy all files that starts with Toolset-llvm-vs2017-xp-x64
- Rename the name of all this files (not the extensions) into Toolset

### LICENSE

Released under Uol-NCSA (Same license as LLVM)
