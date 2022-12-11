1. Foolilng Users: Homographs
	1. use visually similar domain to trick users
	2. Mitigation: browsers use heuristics to block many IDN homographs
2. Fooling Users: Stripping
	1. default to HTTP, MITM makes https request and get response instead
	2. Mitigation: HSTS
		1. Server sends special HTTP header
		2. browser will exclusively use HTTPS for the domain for max-age seconds and not bypass cert errors
		3. HSTS Preload List
3. Fooling Users: Phishing
	1. HTTPS does not prevent that
4. Problems with Site Design
	1. Mixed Content, Cookies, SNI
5. CA Weaknesses
	1. Falsely convince a CA of domain ownership
		1. Mitigation:
			1. limit which CA could issue cert by creating CAA record
			2. Prohibit users creating certain email addresses
			3. introduce multi-perspective validation
	2. Attack on CA:
		1. Example: DigiNotar
		2. CAs can revoke (i.e., cancel) certs they issue by adding them to a Certificate Revocation List (CRL)
		3. Mitigation: Certificate Transparency
			1. Keeping Certificate Transparency log
6. Bugs in TLS implementation
	1. Apple Goto Fail (2014)
	2. Mozilla BERsek (2014)
	3. Null Prefix Attack (2009)
	4. OpenSSL Heartbleed (2014):Vulnerability: OpenSSL trusted user-provided length field and echoed back memory following request data
	5. Mitigation: Formal verification techniques, miTLS is a formally verified TLS library
7. Protocol Vulnerabilities
	1. Compression-related Attacks
	2. Export-grade Cryptography
		1. The FREAK Attack: Deliberately weakened crypto 
	3. Default configuation pitfalls: Mitigation: SSL Labs
	4. Theft of private keys
8. 