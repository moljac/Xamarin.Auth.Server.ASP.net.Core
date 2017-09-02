# Xamarin.Auth.Server.ASP.net.Core

Port of node.js code from "OAuth in Action" to ASP.net Core



## node.js

### Setup

At the begining 

	module.js:442
		throw err;
		^

	Error: Cannot find module 'express'
		at Function.Module._resolveFilename (module.js:440:15)
		at Function.Module._load (module.js:388:25)
		at Module.require (module.js:468:17)
		at require (internal/module.js:20:19)
		at Object.<anonymous> (/Projects/x.a-server/external/OAuth-in-Action-code-nodejs/example/authorizationServer.js:1:77)
		at Module._compile (module.js:541:32)
		at Object.Module._extensions..js (module.js:550:10)
		at Module.load (module.js:458:32)
		at tryModuleLoad (module.js:417:12)
		at Function.Module._load (module.js:409:3)
	
Install packages with `npm`:

	npm install

### Launching Servers
	
	( (node ./client.js &) ; open -a Safari http://127.0.0.1:9000 )
	( (node ./authorizationServer.js &) ; open -a Safari http://127.0.0.1:9001 )
	( (node ./protectedResource.js &) ; open -a Safari http://127.0.0.1:9002 )

	
	tell application "Safari" to open location "http://127.0.0.1:9000"