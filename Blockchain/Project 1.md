

Application that can store information on the blockchain using Solidity in Remix.


We are going to deploy this project on a Javascript VM as we are testing this locally we can make and test the codes faster

Steps involved in [[Buidling Smart Contracts]].
Step 1 : Define your Solidity Version.

'''
pragma solidity ^0.6.0;
'''

^0.6.0 means it will work with any verion of 6 till below 7.
Solidity is a constantly updating language and being good at switching between versions of Solidity is gonna make a powerful Solidity Engineer.

Step 2 : Define a contract

'''
pragma solidity ^0.6.0;

  

contract SimpleStorage {

 uint256 favouriteNumber = 5;

  

}
'''
Here the favouriteNumber will automatically get iniliased to 0.




