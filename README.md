# core2d-skel
Skeleton for [core2d](https://github.com/diogoeichert/core2d), the multi-platform 2D interaction engine

## Usage
It's strongly recommended to use [nvm](https://github.com/nvm-sh/nvm) to manage Node.js versions and [VS Code](https://code.visualstudio.com) for development:

Clone/fork this repository and install dependencies with:
```shell
npm install
```

### Development
Open VS Code and accept the plugin suggestion that will install the Live Preview plugin to make it easier to test your app locally. Right-click the `index.html` file and select "Show Preview" to view the app.

### Building
The app can be built as an Electron app (for desktop operating systems) or as a ZIP file, so that it can be deployed as a mobile or web application.

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
Binaries are created under the `dist/` folder.

#### As ZIP file
```shell
npm run zip
```

### Testing
The electron app can be tested with:
```shell
npm start
```

#### Debugging
You can also open the electron app with the dev console with:
```shell
DEBUG=1 npm start
```

For the web (ZIP) version, please note that modern JS apps cannot be run locally by simply opening the `index.html` file because of [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS). Browsers will need a web server to load the contents of the ZIP file.

It can be conveniently tested with `npx http-server`, though. Just run the command within the expanded folder and open the provided address on the browser.
