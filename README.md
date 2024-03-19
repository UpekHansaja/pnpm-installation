# pnpm-installation

***

### What is a Package Manager?

A package manager is a collection of software tools that automates the process of installing, upgrading configuring, and removing computer programs for an operating system in a consistent manner

Some Examples for Package Managers,
- `npm` (Node Package Manager)
- `yarn` (Yet Another Resource Negotiator) Package Manager
- `pnpm` (Performant Node Package Manager)


`pnpm` installation can be done in several ways,

01. As a Standalone Script.
02. As a npm installation.
03. As a Homebrew installation.
04. As a Choco installation.

### 01. `pnpm` as an Standalong Script

This method helps you to install `pnpm` without any pre install package managers.

If your a Windows (Powershell) User,
```sh
iwr https://get.pnpm.io/install.ps1 -useb | iex
```

If your a POSIX systems User (Linux / UNIX),

```sh
curl -fsSL https://get.pnpm.io/install.sh | sh -
```

</br>

 ---------- [ Mac OS only ] ----------
Now let's Configure Changes we were made,

```sh
export PNPM_HOME="/Users/upekhansaja/Library/pnpm"
case ": $PATH:" in
*": $PNPM_HOME:"*) : ;
*) export PATH="$PNPM_HOME: $PATH" : ;
esac
```

Then to start using pnpm,

```sh
source /Users/upekhansaja/.zshrc
```

***


### 02. `pnpm` via npm installation.

This method helps you to install `pnpm` with the help of `npm`, In here there are 2 package options as follows

- `npm` is a ordinary version of pnpm, which needs Node.js to run.
- `@pnpm/exe` - package which includes NodeJS into an executable.

*If you are prefer to continue with pre-installed NodeJS*

```sh
npm install -g pnpm
```

*or*

*This may be used on systems with **no** Node.js installed.*

```sh
npm install -g @pnpm/exe
```


***


### 03. `pnpm` via Homebrew installation.

If your using Homebrew as your package manager,

```sh
brew install pnpm
```

***


### 04. `pnpm` via Choco installation.

If you have installed Chocolatey,

```sh
choco install pnpm
```

***


*For futher reference visit `pnpm` [installation guide](https://pnpm.io/installation).*