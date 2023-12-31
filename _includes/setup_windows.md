### Prerequisites

#### Terminal / Shell

You may use the pre-installed command line tool _**cmd.exe**_. If you're using `Microsoft Visual Studio` you may instead use the `VS2015 x64 Command Prompt` (64bit) or the `VS2013 x86 Command Prompt` (32bit) (or similar). Both can be found in

    'Start -> All Programs -> Visual Studio 2015'

#### Python

ughub requires _**Python**_ to run (at least version 2.6 should be available, higher is recommended). Please make sure that Python is installed by executing the following command:

    py --version

If it is not installed, please download and install it from

[https://www.python.org/downloads/](https://www.python.org/downloads/)

#### Git

Please also make sure that git is installed on your system and that it can be invoked from your terminal or shell.

#### CMake

You will need _**cmake**_ to generate the build files for your compiler. You may install it from

[https://cmake.org](https://cmake.org)

### Downloading ughub
Please clone the github repository, e.g. by executing the following commands:

    cd %HOMEPATH%
    git clone https://github.com/UG4/ughub

This will download ughub to _%HOMEPATH%/ughub_. You may of course clone the repository to any other location. Simply replace _%HOMEPATH%/ughub_ with your path for the remainder of this introduction.

Please make sure to update your ughub installation from time to time by executing

    cd %HOMEPATH%/ughub
    git pull

### Installing ughub
ughub should run out of the box on Windows. However, in order to execute it from any path, you should add

    $HOME/ughub

to your _**Path**_ environment variable (replace $HOME with the actual path). In order to do so, enter

    SystemPropertiesAdvanced

in your shell. This opens the _System Properties_ dialog and highlights the _Advanced_ tab. Click the _Environment Variables_ button at the bottom of the dialog. This opens a dialog which lets you edit the _**Path**_ variable. Note that paths are separated by a semicolon ';'. If the old value of your Path variable was _SomePaths_, the new content should look somewhat like this:

    SomePaths;C:\Users\YOURNAME\ughub

When you're done, press 'OK' to close the dialog. Make sure to restart your Shell in order to apply the changes.

Autocompletion on windows only works in powershell. To use it, add the line

    C:\Users\YOURNAME\ughub\autocompletions\ughub-completion.ps1

to the file (you might need to create it)

    C:\Users\YOURNAME\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1

If you wish to use it, you need to [allow powershell scripts to execute](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7). Execute the following in an PowerShell session executed as Administrator:

    Set-ExecutionPolicy -ExecutionPolicy Unrestricted

Take a look at [this](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-7#profiles-and-execution-policy) to learn about powershell profiles and execution policy.
