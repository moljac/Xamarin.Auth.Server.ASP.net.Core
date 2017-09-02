# Xamarin.Auth.Server.ASP.net.Core

Port of node.js code from "OAuth in Action" to ASP.net Core



## node.js


	( (node ./authorizationServer.js &) ; open -a Safari http://127.0.0.1:9001 )
	( (node ./protectedResource.js &) ; open http://127.0.0.1:9001 )
	( (node ./client.js &) ; open http://127.0.0.1:9001 )