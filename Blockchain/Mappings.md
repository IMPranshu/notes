declatarion syntax :

```
mapping(string => uint256) public nameToFavouriteNumber;
```


A mapping is a simple data type that “maps” two values. For ex- matching a string (domain name) to a wallet address.

This variable is special because it's called a "state variable" and it's cool because it is stored permanently in the contract’s storage. Meaning anyone who calls the register function will permanently store data related to their domain right on our contract.