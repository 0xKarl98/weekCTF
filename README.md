# Intuition 

Basically the intuition behind this ctf was the easy predicability of {block.numer , block timestamp } since nothing is private on blockchain .



# Grab 


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


 
