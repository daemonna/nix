# VISION

## Ideas from other OS

### OpenBSD

* Kernel

### Linux

* Selinux

### Solaris

* RBAC
* Bootadm
* ZFS

**backwards ABI compatibility**

```
Specific Criteria for Source Compatibility:
1) General Source Code Guidelines for Eligible Applications:
• must be written to comply with the standards as listed in standards(5);
• must not be converting 32 bit applications to 64 bit applications or vice versa;
• must not include Makefiles for building object files from compiled applications to run on
specific platforms;
• must not include 3rd party software libraries (binaries) or other programming interfaces;
• must not include Assembler code in any form.
2) Compiler Guidelines for Eligible Applications:
• must be C and C++ applications;
• must have been compiled with the same compiler and OS version on both the Originating
Platform and the Target Platform;
• must have been compiled using a supported Oracle Solaris Studio compiler on a
supported OS release. 
```

### Package manager

should

* Download or processing can be set to run in parallel.
* Can use multiple versions of the same package
* Support for multiple environments
* Supports multi-user package management: multiple users can share a common Nix store securely, don’t need to have root privileges to install software, and can install and use different versions of a package.

* simple repo server (git-like
* versionning
* modular.. posibility to integrate other pkgs


### Pkg security
```
If a CRITICAL or IMPORTANT security issue is currently open against a package, or a security issue of lower severity has been open for at least 6 months, four weeks before the branch point a procedure similar to long-standing FTBFS will be triggered immediately, with 8 weeks of weekly notifications to maintainers and subsequent orphaning and then subsequent removal from distribution.
```
