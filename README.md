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