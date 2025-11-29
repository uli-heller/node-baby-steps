node-baby-steps
===============

This is a tutorial project for myself to get
some basic knowledge about node and javascript.
At the moment, it may not be beneftial to you
at all!

Preparations
------------

Install NODE. Details: TBD.

Verify the installation:

```sh
$ node --version
v24.11.1

$ npm --version
11.6.2
```

Hello World
-----------

- Folder: [000-hello-world](00-hello-world)
- File: [000-hello-world/hello-world.js](000-hello-world/hello-world.js)
  ```
  console.log('Hello world from Node.js');
  ```
- Run:
  ```
  $ node 00-hello-world/hello-world.js 
  Hello world from Node.js
  ```

Working With MongoDB
--------------------

- Create project directory and cd into it: [010-mongodb](010-mongodb)
- Initialize the node project: `npm init -y` -> creates [package.json](010-mongodb/package.json)
  ```json
  {
    "name": "010-mongodb",
    "version": "1.0.0",
    "description": "",
    "main": "index.js",
    "scripts": {
      "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [],
    "author": "",
    "license": "ISC",
    "type": "commonjs"
  }
  ```
- Install the mongodb driver: `npm install mongodb@latest` -> 7.0.0
  ```diff
  diff --git a/010-mongodb/package.json b/010-mongodb/package.json
  index de1cc83..af704c5 100644
  --- a/010-mongodb/package.json
  +++ b/010-mongodb/package.json
  @@ -9,5 +9,8 @@
     "keywords": [],
     "author": "",
     "license": "ISC",
  -  "type": "commonjs"
  +  "type": "commonjs",
  +  "dependencies": {
  +    "mongodb": "^7.0.0"
  +  }
   }
  ```
  
Links And References
--------------------

- [W3Schools - Node.js Tutorial](https://www.w3schools.com/nodejs/)
- [MongoDB - MongoDB Node Driver](https://www.mongodb.com/docs/drivers/node/current/)
- [dev.to -The final step: How to package a Node.JS application as an exe](https://dev.to/luckynkosi/the-final-step-how-to-package-a-node-js-application-4hol)
- [Amplification -5 Different Tools to Bundle Node.js Apps]( https://amplication.com/blog/5-different-tools-to-bundle-nodejs-apps)
