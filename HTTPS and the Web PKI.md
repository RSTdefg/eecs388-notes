- TLS (Transport Layer Security):
	- Intro
		- is a cryptographic protocol that is layered **above** TCP to provide a secure channel
		- Confidentiality and integrity protection for application data while in transit.
		- Client can authenticate server’s identity
		- Focus on TLS 1.3(RFC 8446)
	- TLS Handshake
		1. Negotiate Crypto Algorithms: 
			1. client provide supported algos, server choose the best
			2. including key exchange algo, signature algo, symmetric crypt algo
		2. Establish Shared Secret
			1. Mutually compute a shared secret.
			2. Diffie-Hellman for forward secrecy.
				1. Derive symmetric keys from shared secret and encrypt and integrity check all further data
			3. Authenticate the Server
				1. Server signs, and client verifies, a hash of the entire handshake transcript to this point.
		- To minimize latency, TLS 1.3 handshake works in one round trip
			- Clever design: Client guesses which key exchange algorithm the server will pick.
- X.509 Certificates:
	- certificate: a message asserting the server’s identity and its public key, signed by a certificate authority (CA)
	- Browser includes a set of public keys for the root CAs
- HTTPS Certificate Ecosystem: public key infrastructure (PKI)