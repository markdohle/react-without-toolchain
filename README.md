# react-without-toolchain

MIT xPro REACT Week 3 Notes: What is a Toolchain

Learn how to ceate a React App [here.](https://reactjs.org/docs/create-a-new-react-app.html)

What is a Toolchain?
A toolchain is a package of programming tools that helps you set up an application and its dependencies easily. This week, you’ll use the create-react-app toolchain.  The best way to understand the value of this toolchain is to review what it’s like to create a React application without one.

Create A New React Application Without A Toolchain
Creating a new React application without a toolchain requires many steps that are confusing for beginners and tedious for experienced programmers. 

The following steps show commands that must be run in the terminal, you’ve likely seen all of these commands before except for `npm`. npm is a package manager for JavaScript. It is a library full of tools and applications that you may need for your application to work. As you build more advanced applications, npm will become a necessity.

Step 1 - Create a new directory and initialize npm

mkdir really-cool-app
cd really-cool-app
npn init

This will create a package.json file for which you can provide the name and version.

 

Step 2 - Install react and react-dom packages

npm install react react-dom

This will create a node_modules folder with all dependent libraries to further add dependency inside the package.json file.

 

Step 3 - Create a .gitignore file, to avoid pushing unnecessary files to GitHub

touch .gitignore

 

Step 4 - Create an app directory that will hold most of your React files

mkdir app

 

Step 5 -  Access the new app directory and generate your first three files

cd app
touch index.js
touch index.css
touch index.html



Step 6 - Install packages that will build and bundle the JavaScript files for usage in a browser

npm install --save-dev @babel/core @babel/preset-env @babel/preset-react
webpack webpack-cli webpack-dev-server babel-loader css-loader style-loader
html-webpack-plugin

After all of these steps, you would still need to edit the Webpack configuration, get the babel-loader to work, and then add the Webpack script to the package.json.

Toolchains Help You Create A React App Easily
A toolchain is a package that creates all the necessary files and dependencies after you run a single command from your terminal. 

To create a new React application with the create-react-app toolchain, you would only need to write the command: npx create-react-app app-name for it to auto-generate all of your files and handle the configurations and dependencies.

npx create-react-app really-cool-app

Toolchains, like create-react-app, also simplify the creation of new files and components. When generating a new file or component, create-react-app will handle any configuration changes or file imports that need to happen for your application to work.

Additional Toolchains
Additional popular toolchains for React include Next.js (Links to an external site.) and Gatsby (Links to an external site.). Toolchains aren't specific to React; however. Other front-end libraries and frameworks, like Angular and Vue, have their own toolchains.

As your project's complexity increases, using a toolchain to help generate new files, test, and build your application will save you considerable time.
