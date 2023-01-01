- Destructive/Nondestructive Entry
- "Locks keep honest people honest"
	- Warded locks: 
		- used since ancient Rome, weak
		- Attack: Cut off protrusions, leaving only the part that actually operates the lock
	- Combination Locks:
		- Inexpensive locks have high error tolerance, only need to try ~2000 combos, can reduce to 8
	- Pin Tumbler Lock (current), invented by Linus Yale
		- The bitting of a key encodes a number
		- The bitting and profile code are sufficient to reproduce the key
	- Tubular Locks:
		- form of pin tumbler lock commonly used when there’s not  enough space for a standard length key
		- Attack: jamming in a soft plastic pen and twisting
- Lock Picking
	- Feeler picking: exploits manufacturing imperfections to open a pin tumbler lock one pin at a 
	- Scrubbing or raking moves many pins at random, in hopes of quickly setting them above the shear line
	- Bumping is a highly effective technique that uses inertia to get all the pins to jump above shear line simultaneously
- Master key systems:
	- Master key systems add a layer of wafers to create a hierarchy of keys
	- Add an additional layer of wafers for another layer in the hierarchy (grand master key
	- Efficient algorithm to deduce master key, given any change key:
		- Say lock has P pins, D possible depths. For each pin position p:  
			1. Create D-1 variants of change key, each  
			differing only in position p. (One for each depth except change key’s)  
			2. Test each key and figure out which one opens the lock. That will be the depth of the master key at p
	- Insight: Each stack of pins operates independently, so any hybrid of master and change key cut depths will open lock
- For important assets, adopt a layered approach to physical security: