# Overview

[![Build Status](https://travis-ci.org/duosecurity/duo_nodejs.svg?branch=master)](https://travis-ci.org/duosecurity/duo_nodejs)

**duo_nodejs** - Duo two-factor authentication for Node.js web applications: https://duo.com/docs/duoweb

This package allows a web developer to quickly add Duo's interactive, self-service, two-factor authentication to any web login form - without setting up secondary user accounts, directory synchronization, servers, or hardware.

Files located in the `js` directory should be hosted by your webserver for inclusion in web pages.

# Installing

Development:

```
$ git clone https://github.com/duosecurity/duo_nodejs.git
$ cd duo_nodejs
$ npm install
```

System:

```
$ npm install global duo_web
```

Or run the following to add to your project:

```
$ npm install --save-prod duo_web
```

# Using

```
$ node --interactive
> const duo_web = require('duo_web');
> duo_web.sign_request(ikey, skey, akey, username);
'TX|...TX_SIGNATURE...==|...TX_HASH...:APP|...APP_SIGNATURE...==|...APP_HASH...'
```

# Test

```
$ npm test
...
OK: 13 assertions (42ms)
```

# Support

Report any bugs, feature requests, etc. to us directly: support@duosecurity.com

