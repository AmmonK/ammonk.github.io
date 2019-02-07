## Ammon's Node/NPM guide

## Mac

_Installing node with the installer on a MAC is not recommended._ It will cause permission errors with globally installed packages and the need to run the SUDO command. A student with the habit of running SUDO on a command to get it to work will cause many issues.

Curriculum uses [Homebrew](https://brew.sh/){:target="\_blank"} to install Node on MAC, which is recommended.

If there are MAC Node/NPM permission issues, here is the easiest fix:
[source](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally){:target="\_blank"}

```
mkdir ~/.npm-global
npm config set prefix '~/.npm-global'

```

add to ~/.bash_profile

```
export PATH=~/.npm-global/bin:$PATH
```

There might still be errors installing packages, this is because NPM cache is now considered to be dirty; it has references to two potential locations.

```
sudo npm cache clean --force
```

All global NPM packages will need to be re-installed into their new location.

## Windows

Use node [installer](https://nodejs.org/en/){:target="\_blank"}.

[Previous versions](https://nodejs.org/en/download/releases/){:target="\_blank"}

## Important commands

List all installed global packages:

```
npm list -g --depth=0
```

Find out where global packages are installed:

```
npm config get prefix
```

Install a global package:

```
npm install -g package_name
```

Uninstall a global package:

```
npm uninstall -g package_name
```

Install a local package:

```
npm install package_name
```

Uninstall a local package:

```
npm uninstall package_name
```

Install all packages from package.json:

```
npm install
```

## Errata

Preferred node management software:

Mac: [nvm](https://github.com/creationix/nvm){:target="\_blank"}

Windows: [nvm-windows ](https://github.com/coreybutler/nvm-windows){:target="\_blank"}
