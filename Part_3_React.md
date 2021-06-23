# Part 3 - React.js

## [Learning JS Together - React (#3)](https://www.youtube.com/watch?v=1DTvRu4pILY)

📺 YouTube Live: <https://youtu.be/1DTvRu4pILY>

---

In this episode, we will be setting up the development tools for Kintone Plug-in Development!

---

## Notes

### Starting Point

[Table-Utility-Plug-in/blob/main/1_Starting_Point/](https://github.com/ahandsel/Table-Utility-Plug-in/blob/main/1_Starting_Point/)
  * [manifest.json](https://github.com/ahandsel/Table-Utility-Plug-in/blob/main/1_Starting_Point/src/manifest.json)

We need to start by reconfiguring the manifest.json file by linking to the appropriate code.

Automate the Kintone Plug-in Development pipeline
  * Details at [Developer_Tools.md](Developer_Tools.md)

### Inside `build` folder

`npm run build` command generates this folder.

Webpack takes in the React JSX files and generates the JS files.

### Build the `manifest.json` file
  * Missing link turn our directory of code into a machine readable
  * Webpack starts from index.js --> then spider their way into all the refereed files
  * Kintone Plug-in's desktop.js & config.js never touch.

### package.json

### Babel is a JavaScript compiler
  * <https://babeljs.io/>

### Setting up enbormental values
Create a `.env` file with the following:

```sh
KINTONE_BASE_URL=<subdomain>.kintone.com
KINTONE_USERNAME=<user name>
KINTONE_PASSWORD=<user password>
```

Add `.env` to `.gitignore` to prevent your Kintone login credential from being uploaded.

### dotenv-cli

`npm install -g dotenv-cli`

[entropitor/dotenv-cli: A cli to load dotenv files](https://github.com/entropitor/dotenv-cli)

Use dotenv to map the Kintone login credential inside `.env` in the command

### cross-var

`npm i cross-var`

[elijahmanor/cross-var](https://github.com/elijahmanor/cross-var)

Use cross-var to make our custom commands usable across Mac, Linux, and Windows


### Create the `pack` command
`npm run pack`

Tie it to kintone-plugin-packer

`--ppk PPK_FILE`: The path of input private key file. If omitted, it is generated automatically into <Plugin ID>.ppk in the same directory of PLUGIN_DIR or --out if specified.

