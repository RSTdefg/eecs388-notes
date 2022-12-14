- Cookie: a piece of data that a server sends to the browser
	- Maintain session state
	- Personalization
	- Tracking
- Same-Origin Policy
	- Enforced by the browser, separate content into different trust domains and restricts data flows between them
	- Origin: scheme+domain+port
	- Isolation: 
		- Cookies
		- DOM Storage and Tree
		- Javascript Namespace
		- Permission to use local hardware
- [[Cookies]] use a different scope than DOM
	- ([scheme], domain)
	- "secure" attribute: limit cookie to HTTPS requests
	- "HttpOnly": A cookie with the `HttpOnly` attribute is inaccessible to the JavaScript [`Document.cookie`](https://developer.mozilla.org/en-US/docs/Web/API/Document/cookie) API; it's only sent to the server
	- Set cookies: for its own domain or any parent domain
	- Read cookies: for its own domain or any parent domain
	- Caution: Cookies also specify a path on the site, but (without HttpOnly) it’s for efficiency only. DOM origins aren’t isolated by path, so scripts can read cookies set for any path in the origin.
- 