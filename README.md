# Remix Plugins for Visual Studio Code
This project aims to provide a similar interface like Visual Studio Code extension manager but for Remix plugins.

For more info on what Remix is and what plugins do please visit our [Remix IDE](https://remix.ethereum.org/) and [Remix Project website](https://remix-project.org/)

## Installation from the Visual Studio Code Marketplace
[Install from VSCODE Marketplace](https://marketplace.visualstudio.com/items?itemName=Ethential.code-remix)


## Requirements

Before being able to use the extension, you need to have at least a folder opened or a workspace.

## The plugins

The extension loads with a default set of plugins. As time goes on we will add more plugins.  The plugin system allows developers to access and interact with the file system and other components, plugins and extensions.

You can also suggest and create plugins using our plugin system and API. Feel free to contact us on our gitter channels.
[Remix](https://gitter.im/ethereum/remix) & [Remix Dev](https://gitter.im/ethereum/remix-dev)
## Select, activate, deactivate plugin

![Activate, deactivate remix plugin](https://j.gifs.com/3QMVnM.gif)

## Load a development plugin

* Click on add plugin button from `Remix Plugins More actions` menu on top right
<p align="justify">
  <img src="https://user-images.githubusercontent.com/13261372/101530235-a5e55280-39b7-11eb-820d-99ada3ae1f33.png" height="273">
</p>

* Add your `JSON` plugin info into the input box. An example is given below.
```json
{
  "name": "solhint-dev",
  "displayName": "Solhint development",
  "methods": [],
  "version": "0.0.1-dev",
  "url": "/home/0mkar/Karma/remix-solhint-plugin",
  "description": "Run Solhint in your Remix project",
  "icon": "https://raw.githubusercontent.com/protofire/solhint/master/solhint-icon.png",
  "location": "sidePanel"
}
```
<p align="justify">
  <img src="https://user-images.githubusercontent.com/13261372/101530718-4b002b00-39b8-11eb-885b-d42e6b1352ad.png" height="434">
</p>

* Upon enter you will see your development plugin on the activiety toolbar.
<p align="justify">
  <img src="https://user-images.githubusercontent.com/13261372/101531113-d37ecb80-39b8-11eb-877d-99c0d0c474c8.png" height="431">
</p>


## Development
```
yarn
code .
[start plugin with F5]
```