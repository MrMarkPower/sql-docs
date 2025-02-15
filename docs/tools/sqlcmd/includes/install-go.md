---
author: rwestMSFT
ms.author: randolphwest
ms.date: 08/15/2023
ms.service: sql
ms.topic: include
---
**sqlcmd** (Go) can be installed cross-platform, on Microsoft Windows, macOS, and Linux.

### [Windows](#tab/windows)

#### winget (Windows Package Manager CLI)

1. Install the [Windows Package Manager Client](/windows/package-manager/winget) if you don't already have it.
1. Run the following command to install **sqlcmd** (Go).

   ```bash
   winget install sqlcmd
   ```

#### Chocolatey

1. Install [Chocolatey](https://community.chocolatey.org/) if you don't already have it.
1. Run the following command to install **sqlcmd** (Go).

   ```bash
   choco install sqlcmd
   ```

#### Direct download

1. Download the corresponding `-windows-x64.zip` or `-windows-arm.zip` asset from the [latest](https://github.com/microsoft/go-sqlcmd/releases/latest) release of **sqlcmd** (Go) from the GitHub code repository.

1. Extract the `sqlcmd.exe` file from the downloaded zip folder.

### [macOS](#tab/mac)

#### Homebrew

1. Install Homebrew if you need to.

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

1. Install **sqlcmd** with Homebrew.

    ```bash
    brew install sqlcmd
    ```

#### Direct download

1. Download the `-darwin-x64.zip` asset from the [latest](https://github.com/microsoft/go-sqlcmd/releases/latest) release of **sqlcmd** (Go) from the GitHub code repository.

1. Extract the `sqlcmd` file from the downloaded zip folder.

### [Linux](#tab/linux)

#### apt (Debian/Ubuntu)

1. Import the public repository GPG keys.

   ```bash
   curl https://packages.microsoft.com/keys/microsoft.asc | sudo tee /etc/apt/trusted.gpg.d/microsoft.asc
   ```

1. Add the Microsoft repository, where the `ubuntu/20.04` segment may be `debian/11`, `ubuntu/20.04`, or `ubuntu/22.04`.

   ```bash
   add-apt-repository "$(wget -qO- https://packages.microsoft.com/config/ubuntu/20.04/prod.list)"
   ```

1. Install **sqlcmd** (Go) with **apt**.

   ```bash
   apt-get update
   apt-get install sqlcmd
   ```

#### yum (Fedora/CentOS)

1. Import the Microsoft repository key.

   ```bash
   rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

1. Download the repository configuration file, where the `centos/8` segment may be `centos/8`, `fedora/32`, `opensuse/42.3`, `rhel/8`, or `sles/15`. If the version of your OS doesn't directly correspond to one of those options, you can likely successfully use a repository configuration file from a version. For example, `centos/8` can be used in an environment running CentOS 7.

   ```bash
   curl -o /etc/yum.repos.d/packages-microsoft-com-prod.repo https://packages.microsoft.com/config/centos/8/prod.repo
   ```

1. Install **sqlcmd** (Go) with **yum**.

   ```bash
   yum install sqlcmd
   ```

#### Direct download

1. Download the corresponding `-linux-x64.tar.bz2` or `-linux-arm.tar.bz2` asset from the [latest](https://github.com/microsoft/go-sqlcmd/releases/latest) release of **sqlcmd** (Go) from the GitHub code repository.

1. Extract the `sqlcmd` file from the downloaded zip folder.

---
