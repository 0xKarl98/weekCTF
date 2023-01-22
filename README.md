# Intuition 

Basically the intuition behind this ctf was the easy predicability of {block.numer , block timestamp } since nothing is private on blockchain .

Note that the transfer method is not secure at current existing blockchain world , as the underlying SSload instructions gas cost can be changed , 

which is vulnerable for an re-entrancy attack .


# Run the attacker inside test folder 

Firstly fork the goerli network inside a block , using 
```
ganache --fork.network goerli
```
Then run the test inside test folder 
```
forge test --match-contract PrivateDataTest --fork-url <your_rpc_url> --fork-block-number 7178864 -vv

```
where you can grab your own rpc_url from Alchemy provider .


 
