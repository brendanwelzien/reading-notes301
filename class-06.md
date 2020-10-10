## Introduction to Node.JS
- Node.js is an event-based, asynchronous, non-blocking running program that uses engines and libraries
    - it is built into Google Chrome's V8 JS engine
    - the 'V8 engine' is the open-source JS engine that runs in Google Chrome, it is responsible for compiling code for execution.
- Node.js is a program that can be executed on computers and not in the browser.

- When downloading Node.js, it is recommended to download the version manager so you can install multiple versions and switch at will (per-project basis)
    - check if downloaded by using `node -v` and it should show the *version*
        - Node.js is highly beneficial in negating *compatibility issues*
## NPM
- NPM is a package manager that comes along with Node.js
    - largest software base
    - installing a package *globally* = `npm install xxx`
    *locally* = `npm init -y`

## Working with a package.json file
- if you look at contents of a directory, you'll notice a folder called `node_modules`
    - this is where npm has saved information, and should be re-created any time by running npm install from the project root
    - the `dependencies` field allows any developer to clone your project and use npm install for packages needed to run
## Usage of Node.js
- designed to automate JS application development process
- lets us run JS on the server
- *event-driven*, everything happens in Node.js is in reaction to events
1. Node adds pass async tasks to evet loop with a callback (funciton, callback)
2. event loops manages a thread pool and executes tasks
3. executes each callback as tasks complete

[<=Back](README.md)