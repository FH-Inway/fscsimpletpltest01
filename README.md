# Simple GitHub repository template for D365 FSCM projects

This repository template is a starting point for D365 FSCM Extension projects. It covers the repository setup and running a build on the repository. More advanced scenarios are covered by other FSC-PS templates.

To learn in general on how to set up this repository template, visit [FSC-PS for GitHub](https://github.com/fscpscollaborative/fscps).

## Template specific instructions

[FSC-PS for GitHub](https://github.com/fscpscollaborative/fscps) provides you with general information on how to set up this and other FSC-PS templates. In addition, there is some setup specific to D365 FSC Extension projects. 

### Install the repository code

To make the D365 FSCM extensions from this repository available in the D365 FSCM application of a development environment, the repository needs to be installed in a particular way. To do this, run [Install-RepositoryCode.ps1](Install-RepositoryCode.ps1) as follows:
- Connect to your development environment using Remote Desktop.
- Download the [Install-RepositoryCode.ps1](Install-RepositoryCode.ps1) script.
- Run the script in a PowerShell session with administrator permissions.
- The script will ask for a name and email address for the Git configuration.
- It will also ask for the URL of the repository to clone. You can find that URL on GitHub by clicking the green "Code" button and copying the URL.


### Add a D365 FSCM module

Now you can use Visual Studio as you normally would to create a new D365 FSCM module or install an existing one. Once that is done, the source code files of the module will appear as new file changes in Git. Those changes can be [committed](https://learn.microsoft.com/en-us/visualstudio/version-control/git-make-commit) and [pushed](https://learn.microsoft.com/en-us/visualstudio/version-control/git-push-remote) from within Visual Studio to the repository on GitHub.