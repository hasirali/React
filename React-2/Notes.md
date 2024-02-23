# Creating Package.Json

``` npm init ```
and
````npm init -y````
if want to make fast

#

```
Package.json is the configuration for npm and 
specifies project metadata and dependencies

<!-- why we need: -->
npm wil take care of version of package and where it takes it takes in package.json

so we dont need to put nodemodule in github and we can stop it by writin node_module in gitignore also add parcel-cahce and dist folder as all these can regenerated

<!-- our project is dependent on lots of dependencies or package 


```
most important package is bundler , job:bundler your app or package your app so it can ship for production example vite and parcel ,webpack.

```{
  "name": "react2",
  "version": "1.0.0",
  "description": "making na understanding Basics of react and npm",
  "main": "index.js",
  "scripts": {
    "test": "jest"
  },
  "keywords": [
    "react",
    "reactjs"
  ],
  "author": "Hasir Ali",
  "license": "ISC"
}
```

# Package-lock.json

locks the version and keeps the record of ecevry exact package.

records the exact versions of dependencies to ensure consistent installations across different environments. The latter is generated automatically when npm installs or updates packages, ensuring reproducibility in dependency versions.

# NodeModules
A "node_modules" directory is created in a Node.js project when you use npm (Node Package Manager) to install dependencies for that project. This directory contains the libraries and packages (node modules) that your project depends on. Each installed package is typically represented by a folder within "node_modules," and it includes the package's code and any other necessary files. 

and every package has its own package.json
#
# Working with Parcel
first of all there are two dependencies : dev dependencies[-D](genrally required for developmet) and Normal Dependencies(use for production)




Parcel Gives
- HMR or Hot Reloading= Hot Module Replacement:File Watching Algorithm - written in C++
- -Caching
- Faster Builds
- Dev Build
- Locat Server
- Image Optimization
- Minification
- Bundling
- Compress
- Consistent Hasihng
- Code Splitting
- Differnetial Bundling (support older browser)
- Diagnostic 
- Error Handling
- Also give enviroment for https
- Tree Shaking Algorithm(remove unused code)

# configuration

```
npm install parcel
<!-- but we are in devlopment we will use  -->

npm install -D parcel

npx parcel index.html

npm install react
npm install react-dom
```

# Extra
``` 
^(caret):Automatically update the package , 
~(Tilde): Install the Major function
```

```
npm: is primarily used for managing and installing packages (dependencies) for a project.

npx:eXcecute is used to execute packages without installing them globally. It allows you to run packages directly from the npm registry without installing them first.

HMR: hot module Replacment(automaic run as we change the code) with help of file watching algorithm writen in c++
every time faster every time built (by caching-u can see in Parcel-cache)

<!-- npx build -->
it will bundle ,minified and put inside dist folder and the ouptput is cooming from dist folder and push so user can use as it size is low dont take much time
```