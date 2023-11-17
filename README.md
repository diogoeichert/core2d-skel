# core2d-skel
Skeleton for the multi-platform 2D interaction engine

## Usage
It's strongly recommended to use [nvm](https://github.com/nvm-sh/nvm) to manage Node.js versions and [VS Code](https://code.visualstudio.com) for development:
### Installation
#### macOS
```shell
brew install nvm
brew install --cask visual-studio-code
```
#### Linux/Windows
Please refer to the links above and check installation options.

Clone this repository and install dependencies with:
```shell
npm install
```

### Development
Open VS Code and accept the plugin suggestion that will install the Live Preview plugin to make it easier to test your app locally. Right-click the `src/index.html` file and select "Show Preview" to view the app and optionally open it in a separate browser window.

### Building
#### As ZIP file
```shell
npm run zip
```

#### As Electron app
```shell
npm run build # all supported platforms
```
##### Linux
```shell
npm run build:lin
```
##### macOS
```shell
npm run build:mac
```
##### Windows
```shell
npm run build:win
```
