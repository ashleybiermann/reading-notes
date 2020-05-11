### Node, Express, and APIs
[An Introduction to Node.js on sitepoint.com](https://www.sitepoint.com/an-introduction-to-node-js)
* * *
**definitions**
- Node.js homepage - Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
- Stack Overflow - Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
- This site - a JavaScript runtime
**V8 engine** open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers
> responsible for compiling JavaScript directly to native machine code that your computer can execute
**Version manager** program that allows you to install multiple version of Node and switch between them 
* * * 
Installing Package Locally
>`npm init -y` creates and autopopulates a `package.json` file
>**dependency** for example, `npm install lodash --save` installs lodash package and saves it as a project dependency
>Contents of directory should have folder named `node_modules` This is where npm has saved lodash and any libraries that lodash depends on
>`npm install ` can be used to recreate `node-modules` folder at anytime. Just run it from the project's root directory 
* * * 
What is Node.js and npm Used For?
- installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.
>running JS on the server!
>bundling your JavaScript files and dependencies into static assets
>running tests 
>automatic code linting and style checking.
>and more...
- developing apps with any modern JavaScript framework (for example, React or Angular?
>expected to know Node and npm, because these frameworks are available via npm and rely on Node to create sensible development environment
* * *
Node.js Lets Us Run JS on the Server 
- Node.js is *single threaded* and *event-driven* - everything that happens in Node is in reaction to an event
- Node uses liblus library to implement asynchronous (non-blocking) behavior
