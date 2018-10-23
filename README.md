# Converse.js Electron App Experimental

This is an Electron.js application which combines Converse.js XMPP client with Node.js based BOSH instance which allows you to use Converse.js just like any other desktop XMPP client.

In order to try out the application:

1. Clone the repository and `cd` there

2. Install dependencies with:

```
npm install
./node_modules/.bin/electron-rebuild --module-dir node_modules/node-expat
```

**Warning**: while electron.js uses its own version of Node.js, initial `npm install` still runs Node version installed on your system and fails for Node `>= 10.x`. You have to run the initial `npm install` with Node version `<= 9.x`, but you don't depend on this after you have done it.

Also, `libgconf-2.4` must be installed on your system (a dependency of Chrome/Chromium).

3. Then run the application:

```
npm start
```
