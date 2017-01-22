# meteor-reactjs-basic
Basic setup for Meteor and ReactJS using Visual Studio Code. By the end of this setup, we will have a proper development environment for working with Meteor, ReactJS, and MongoDB.

Our final objective will be to have a working Simple To-Do application following the following tutorial by Meteor using React. [Tutorial](https://www.meteor.com/tutorials/react/creating-an-app)

# Environment Setup
## 1. Set up Visual Studio Code for Mac
[Download for Mac, stable build.](https://code.visualstudio.com)

Visual Studio Code Recommended Extensions
- vscode-icons by Roberto Huertas
- jslint by Andrew Hyndman
- vscode-pandoc by DougFinke [(link)](http://pandoc.org/installing.html)
- ESLint by Dirk Baeumer

```bash
## JSlint: Run the following in project folder if meets error
$ sudo npm install -g jslint

## ESLint: Run the following in project folder
$ npm install eslint
```

Set up Visual Studio Code Debug [(link)](https://code.visualstudio.com/docs/editor/debugging)

## 2. Set up iTerm for Mac
[Download for Mac, stable release.](https://www.iterm2.com/index.html)

## 3. Set up nodeJS for Mac
[Download for Mac, recommended for most users.](https://nodejs.org/en)

## 4. Meteor Setup
Installation Guide by Meteor [(link)](https://www.meteor.com/install)

Run the following in your terminal or iTerm.
```bash
## Install Meteor
$ curl https://install.meteor.com/ | sh

Meteor 1.4.2.3 has been installed in your home directory (~/.meteor).
Writing a launcher script to /usr/local/bin/meteor for your convenience.

To get started fast:

  $ meteor create ~/my_cool_app
  $ cd ~/my_cool_app
  $ meteor

Or see the docs at:

  docs.meteor.com
```

# Project Setup
Assuming that Run the following in your terminal or iTerm.
```bash
## Create tutorial simple-todos app
$ meteor create simple-todos

## Navigate into the app folder and install node 
$ cd simple-todos
$ meteor npm install

## Run server
$ meteor
```

Go to http://localhost:3000 to test your first Meteor application.

# Simple To-Do application

***Important Note:*** 

*For your application to run, please keep the terminal running the "meteor" command open. This will ensure that your server is still running. You need the server to run your application.*

Go to the terminal running the server and stop the server with CTRL+C. Run the following to install React into your Meteor application.

```bash
## Install React
$ meteor npm install --save react react-dom

## Run your server
$ meteor
```

If you meet the following errors, just stop your server with CTRL+C, and run the following.

```bash
Unable to resolve some modules:

  "react" in /Users/kirene/Documents/github/meteor-reactjs-basic/simple-todos/imports/ui/App.jsx
(web.browser)
  "react-dom" in /Users/kirene/Documents/github/meteor-reactjs-basic/simple-todos/client/main.jsx
(web.browser)

## Install React again. Ensure that you stopped the server before installation.
$ meteor npm install --save react react-dom

## Run your server
$ meteor
``` 
With these, you should be able to go through the [simple to-do application tutorial](https://www.meteor.com/tutorials/react/creating-an-app) without any problem. 