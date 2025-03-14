# NPM Commands Cheatsheet

## ✅ Checking NPM Version

```sh
npm -v  # Check the installed NPM version
```

## ✅ Installing NPM (If not installed)

- NPM comes with Node.js. To install it, download and install Node.js from [nodejs.org](https://nodejs.org/)

## ✅ Initializing a Project with NPM

```sh
npm init  # Starts an interactive process to create a package.json file
npm init -y  # Creates package.json with default values
```

## ✅ Installing Packages

```sh
npm install package-name  # Install a package locally (to node_modules)
npm install -g package-name  # Install a package globally
npm i package-name  # Shorter version of install command
npm i package-name@version # Install a specific version of the package you want
npm i package-name --save-dev # Install a package as a development dependency package only
```

## ✅ Installing All Dependencies (From package.json)

```sh
npm install  # Installs all dependencies listed in package.json
```

## ✅ Removing Packages

```sh
npm uninstall package-name  # Removes a package
npm uninstall -g package-name  # Removes a globally installed package
npm un package-name # Removes a package (un is an abbreviation for uninstall)
npm remove package-name # Removes a package
npm rm package-name # Removes a package (rm is an abbreviation for remove)
```

## ✅ Updating Packages

```sh
npm update package-name  # Updates a specific package to the latest version
npm update  # Updates all dependencies to their latest allowed versions
```

## ✅ Checking for Outdated Packages

```sh
npm outdated  # Shows outdated packages with available updates
```

## ✅ Running Scripts (Defined in package.json)

```sh
npm run script-name  # Runs a custom script defined in package.json
```

Example (if package.json contains a script like this):

```json
"scripts": {
  "start": "node index.js"
}
```

Run it using:

```sh
npm run start
```

## ✅ Managing Dependencies

```sh
npm list  # Lists installed dependencies
npm list -g  # Lists globally installed dependencies
npm list --depth 0 # Lists only only installed dependencies in depth 0 of the dependency tree
npm ls package-name  # Shows details of a specific package
```

## ✅ Installing Dev Dependencies

```sh
npm install package-name --save-dev  # Installs a package as a dev dependency
```

## ✅ Set and Get configs

```sh
npm config set init-author-name "Parsa"  # From now on, everytime that `npm init -y` command is executed, package.json file will have the author's name specified as Parsa. another example:
npm config set init-license "MIT" # From now on, everytime that `npm init -y` command is executed, package.json file will have the license specified as MIT
npm get init-license # Shows you the license name
```

## ✅ Clearing Cache

```sh
npm cache clean --force  # Clears NPM cache
```

## ✅ Checking Package Security Issues

```sh
npm audit  # Scans dependencies for vulnerabilities
npm audit fix  # Attempts to fix security vulnerabilities automatically
```

## ✅ Uninstalling and Reinstalling All Dependencies

```sh
rm -rf node_modules package-lock.json  # Removes all installed dependencies
npm install  # Reinstalls dependencies
```

## ✅ Showing Package Info

```sh
npm view package-name  # Shows package details from the registry
npm show package-name  # Alias for npm view
```

## ✅ Linking Global Packages Locally

```sh
npm link package-name  # Links a globally installed package to local node_modules
```

## ✅ Running NPM in Different Modes

```sh
npm ci  # Installs dependencies exactly as listed in package-lock.json (faster and deterministic)
```

## ✅ Publishing a Package to NPM

```sh
npm login  # Log in to NPM
npm publish  # Publish package to NPM registry
```

## ✅ Ignoring Files When Publishing

- Add a `.npmignore` file to exclude files from being published.

---

### 📌 Created with ❤️ by Parsa Hosseii

