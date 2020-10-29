# Creating a React App from Scratch

Based on [this article](https://blog.usejournal.com/creating-a-react-app-from-scratch-f3c693b84658) with some updates for new versions of packages. 

The following are the commands I used to create the application structure: 
```bash
% npm init
% git init .
% mkdir public src
% touch .gitignore
% npm install --save-dev @babel/core @babel/cli @babel/preset-env  @babel/preset-react 
% touch .babelrc
% npm install --save-dev webpack  webpack-cli webpack-dev-server  style-loader css-loader babel-loader
% npm install react react-dom
% npm install react-hot-loader
```

Note that I've removed the version numbers (eg. webpack@5.3.1) from the package names. This
is because that article is from two years ago and these packages will have been updated since
it was written. I wanted to install the latest version of all of these packages so leaving 
off the version number achieves this.   The danger here is that I get incompatible versions 
of some packages.

Run server with:

```bash
% webpack serve --mode development
```

(note not `webpack-dev-server` any more)