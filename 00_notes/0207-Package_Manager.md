# General
- Package -> compresses archive containing all required files
  - packages have dependencies that generally aren't package
- Package managers resolve the dependencies of packages
- They know where to put all parts of the packages in the Linux File-System

# APT vs APT-GET vs SNAP
- apt is a newer version of apt-get that bundles more commands for better user
  experience
- snap is an alternative package manager
    - while it does resolve dependencies it doesn't install them separately but
      bundles them with the package. apt installs them separately so that
      dependencies can be shared amongst different packages.
- snap supports automatic updates
- snap supports universal linux images whereas apt (apt-get) only supports .deb
  packages for debian based distributions

=> prefer apt

# Adding Custom Repositories
- PPA (Personal Package Archive)
- Custom Community maintained repositories
- They're not verified by Linux Distros, which implies security risks
- Certain software (like docker on debian systems) is not available in the
  standard repositories, therefore we need to add repositories

# 
1. Debian Based (e.g. Debian, Ubuntu)
    - uses apt
2. Read-Hat based (RHEL, CentOS, Fedora)
    - uses yum as package manager
    - the concept is very similar to apt or other package managers

Depending on the distribution different repositories are included by default.
