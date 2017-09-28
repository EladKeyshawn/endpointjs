![alt text](https://github.com/EladKeyshawn/endpoint-js/blob/master/assets/road-detours.png)
# endpoint.js
[![NPM](https://nodei.co/npm/endpoint-js.png)](https://npmjs.org/package/endpoint-js)
---

> Simplistic express routing management for NodeJS

- Manage all endpoints in a structure file
- Controller and routers folders and files are created automatically by route
- Built in CLI for creating boilerplate and adding new endpoints
- Automatically registers your (Endpoint | Router | Controller) with express 

## Install

> CLI
```
$ npm install --global endpoint-js
```

> endpoint.js
```
$ npm install --save endpoint-js
```

## Usage

In your home directory create endpoint app boilerplate:
```
$ endpoint --i
```
And your api routing folder and ready!

// screenshot

To add an API route (Endpoint)
```
$ endpoint --a
```
fill in the prompt with your endpoint details, for example:
- endpoint path: /api/is/awesome
- router file name: awesome.js
- controller file name: awesomeController.js
// screenshot


And an endpoint was added to Router.js (API structure file),
foldering and file creation is done automatically!


In your index.js or wherever you create your express app, simply:
```js
var app = express();
require('endpoint-js')(app);
```

OPTIONALS:

- if you want all of your endpoint structure to have some predetermined 
prefix you can do so:
```js
require('endpoint-js')(app, {prefix: "/someprefix"});
```


##### LICENCE & CREDITS
MIT © [Elad Keyshawn](https://github.com/eladkeyshawn)
