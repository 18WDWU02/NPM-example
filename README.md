# Node Package Manager (NPM) Example

An example of how to use NPM in your project.
All dependencies aren't included in the repository because of the .gitignore file.

### Installation of this repository

This project requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies from the package.json file to successfully run the project

```sh
$ cd NPM-example
$ npm install
```
### Installation of NPM
To install npm in your project you first need to have a valid version of nodejs on your computer/server.
```sh
$ cd project_name
$ npm init
```
Follow the prompts it gives you. It will then create a package.json file for you in your project.
The package.json file includes all the dependencies needed for your project to run. Because you are using NPM, these dependencies don't need to be sent up to git. So make sure to ignore the node_modules folder in your .gitignore.

### Installing a package
Find the package you want to include from the [NPM site](https://www.npmjs.com/).
When you have found the package you want type in
```sh
$ npm install package_name --save
```
This adds the package onto your package.json file and also adds all the required folders in the node_modules folder.

### Updating a package
If a new version of a package comes out, all you need to say is
```sh
$ npm update
```
This reads your entire package.json file and searchers for the latest versions for all the dependencies which have the caret symbol (^) before the version number. The caret stands for the latest version higher than the version number given.

### Removing a package
You don't want to manually remove the packages from the node_modules folder. And often one dependency includes multiple folders. To remove any package you just call
```sh
$ npm remove package_name --save
```
This removes the dependency from the package.json file as well as the node_modules folder. It won't remove any instances of it throughout the project though.
