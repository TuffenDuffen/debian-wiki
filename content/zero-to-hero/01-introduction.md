+++
title = '01 Introduction'
date = 2026-06-05T13:04:57+02:00
+++
## Debian is an operating system

Debian is a free and open-source operating system.

Debian is a Linux operating system, meaning that software for Debian can be configured to work for other Linux operating systems, and vice versa (in most cases, we will expand on this later).

Linux operating systems are usually called **distributions** or **distros** for short. They comprise many independent components, such as a login screen, firewall, file manager, notepad, audio playing system, and window handling system, orchestrated to deliver a cohesive user experience.

## Debian's package manager

The independent components of a distribution are distributed as **packages**

Most Linux distributions contain tools to install new components, update or remove installed components and create brand new components. These are usually called **package managers**. Some distros share package manager with another, only changing the pre-installed components.

Debian's package manager is called APT. This is the same package manager as the one found in Ubuntu, Linux Mint, and Pop!_OS to name a few. This means that most software for Debian is available in these distros, and vice versa. However, these other distros may use other **repositories**, collections of installable packages, based on what works for their purposes.

Some other system package managers are Arch's pacman, Fedora's DNF and openSUSE's zypper

### The Linux package management ecosystem

In the Linux world, most well-written software can on all major distros, and there is much overlap between the package managers. However, some distros are more hesitant to package and distribute a brand-new release of some software, and want to wait until the release is properly and thoroughly tested. Debian is the most hesitant, leading to Debian packages being several releases behind while for example Arch has the latest release.

Also, most Linux programs use *libraries* which contain common functionality in order to not have to reinvent the wheel. In order to conserve user disk space and decrease package reconfiguration times when updating a frequently used library, for example in the case of a security vunerability, distros commonly only ship one version of a library and wait with shipping new versions of programs until the libraries they depend on are updated, which in the case of non-backwards compatible updates may take a while.

This creates a stream of versions trickling downwards from the bleeding-edge to the more stable distros.

This also means that software from repositories with more recent versions of libraries may be incompatible with software from other repositories, even though they use the same package manager. This is the case of Ubuntu, which updates more frequently than Debian, causing some software available for Ubuntu not to being compatible with Debian.
