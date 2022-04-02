# Zero Address

The zero address in Solidity is sort of like the void (in the literal sense) where everything comes from. When an address mapping is initialized, all entries in it point to the zero address.

So if a domain hasn’t been registered, it’ll point to the zero address!

ex-
```
require(domains[name] == address(0));
```