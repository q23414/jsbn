**Core Library**

`jsbn.js` - basic BigInteger implementation, just enough for RSA encryption and not much more.

`jsbn2.js` - the rest of the library, including most public BigInteger methods.

**RSA**

`rsa.js` - implementation of RSA encryption, does not require jsbn2.js.

`rsa2.js` - rest of RSA algorithm, including decryption and keygen.

**ECC**

`ec.js` - elliptic curve math, depends on both jsbn.js and jsbn2.js

`sec.js` - standard elliptic curve parameters

**Utilities**

`rng.js` - rudimentary entropy collector and RNG interface, requires a PRNG backend to define prng_newstate().

`prng4.js` - ARC4-based PRNG backend for rng.js, very small.

`base64.js` - Base64 encoding and decoding routines.

`sha1.js` - SHA-1 hash function, only needed for IBE demo.