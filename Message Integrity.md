
- Ensures that attackers cannot modify messages without being detected
- Message Verifier: 
	- Random Function
		- Giant lookup table, provably secure but impractical
	- Pseudorandom Function
		- Functions all known to Mallory, choose n-bit index key known only to recv, sender
	- Cryptographic Hashes
		- Fixed function, no key
		- Properties:
			- Preimage resistance:Given output h, hard to find input m s.t. h = H(m)
			- Second-preimage resistance:Given input m1 , hard to different m 2 s.t. H(m1 ) = H(m2 )
			- Collision resistance:Hard to find any pair of inputs m1 ,m 2 s.t. H(m1 )=H(m2 )
		- Examples:
			- Insecure: #MD5 #SHA-1
			- Secure: [[SHA-256]], SHA-512, SHA-3
- Psudorandom Generator #PRG 

#### 

### 

##