# IWLTech Utils
## Utilities for managing your Fedora system quickly and efficiently.

### Usage and Installation

To install, simply clone this repository, make install-now executable, then run it. The usage is printed after install when you run iwltech.

#### Dependencies
    dnf
    bash
    basic utilities such as git, grep, cut, mv, cp, cd, mkdir, sudo, chmod, tar
You will have all you need on a fresh Fedora Workstation operating system.

### Features
    Usage:
        iwltech [GLOBAL OPTIONS] <COMMAND> [ARGUMENTS] [COMMAND-SPECIFIC OPTIONS]
    
    Description:
        IWLTech Utils is a program for managing several areas of your system. It also aims to make Linux easier for beginners.
    
    Commands:
        maintenance                       Run the maintenance script.
        post-install                      Run the post-install script.
        config                            Edit a command's configuration with questions. Takes -r for the command.
        
    Commands requiring an attribute:
        package-search                    Search the package databases for package named by the attribute.
        package-install                   Installs a package named by the attribute.
        package-uninstall                 Uninstalls a package named by the attribute.
        package-update                    Updates a package named by the attribute. If no attribute supplied, updates the system.
    
    Aliases:
        main                              Alias for 'maintenance'.
        pi                                Alias for 'post-install'.
        3.141592653589793238462643383     Alias for 'post-install'.
        ps                                Alias for 'package-search'.
        search                            Alias for 'package-search'.
        install                           Alias for 'package-install'.
        i                                 Alias for 'package-install'.
        pu                                Alias for 'package-uninstall'.
        uninstall                         Alias for 'package-uninstall'.
        u                                 Alias for 'package-uninstall'.
        update                            Alias for 'package-update'.
        up                                Alias for 'package-update'.
        upgrade                           Alias for 'package-update'.
    
    Global options:
        -c=[arg], --config=[arg]          Use the configuration file specified in the argument. 
        -h, --help                        Print help
        -v, --verbose                     Print all results of commands to the terminal.
        -o, --ok, --okay                  Ask for confirmation before performing an action.
        --dangerous                       Allow the use of dangerous commands.
        --installer                       Open the installer to reinstall, update or uninstall.
        
    Packager options (for use with package-* commands):
        -f, --flatpak, --flatpak-only     Use flatpak packages only.
        -d, --dnf, --dnf-only             Use dnf packages only.
    
    Command specific options for config:
        -r=[arg], --read=[arg]            The command to edit the configuration of.
        
    Command specific options for package-update:
        -l, --list, --list-only           Only list the packages that need updating, do not update them.

### Roadmap
    
#### Release V2

Add post-install
    
#### Release V3

Add custom tailored configs for maintenance and post-install
    
#### Release V4

Add logs feature
    
#### Release V5

Sort search package results and streamline package jumps for search & check-update
    
#### Release V6

Sort check-update results
Colour outputs
    
#### Release V7

Add intelligent search to the package manager (install & uninstall) (searching dnf & flatpak, if only one exists, run on it, otherwise prompt)
    
#### Release V8

Add autorun for keyboard shortcuts.
    
#### Release V9

Add schedule and timer options, and their configs.

### Copyright

The code in this repository is hosted and created by IWLTech. It is licensed under the "I HATE AI LICENSE" (https://github.com/IWLTechnology/project-licences/blob/main/I_HATE_AI_LICENSE). Feel free to modify and remix as long as it abides by the license. The Linux utilities used in this script are licensed differently, and this license does not override it.
