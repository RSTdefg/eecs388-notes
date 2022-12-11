
- Ensures that attackers cannot modify messages without being detected
- Message Verifier: 
	- Random Function
		- Giant lookup table, provably secure but impractical
	- Pseudorandom Function
		- Functions all known to Mallory, choose n-bit index key known only to recv, sender
	- Cryptographic Hashes
		- Fixed function, no key
		- Properties:
			- Preimage resistance
			- Second-preimage resistance
			- Collision resistance
		- Examples:
			- Insecure: #MD5 #SHA-1
			- Secure: [[SHA-256]]
- Psudorandom Generator #PRG 

#### 

### 

##