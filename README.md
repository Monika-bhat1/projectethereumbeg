# MyToken

This project is based on creeating a token using the solidity language that is a high level language.This project allows us to create a smart contract that allows to implement various concepts such as mapping, storing, destroying the tokens created. It also maintains the condition that we burn the amount of fas that we have and not more than that. 

## Requirements

1. Accoding to the first requirement mentioned in the assessment, the contract has public variables that store the details about the coin:
     1.tokenName: A string representing the name of the token.
     2.abbrv: A string representing the abbreviation of the token.
     3.totalSupply: An unsigned integer representing the total supply of the token as it cannot be negative.

2. The second requirment of the assessment requires the contract has a mapping of addresses to balances:
     1.balances: A mapping that associates addresses with their corresponding token balances.
     Whenever we enter a address to the deployed contract, it tells us about the value associated with it,that is, the token balance.

3. The contract has a `mint` function that increases the total supply and the balance of the "sender" address by a given value:
     It accepts the Parameters:
      1. _address: The address to which the tokens will be minted.
      2. _value: The amount of tokens to be minted.
   The mint function performs the following actions when the parameters are passed:
      1.Increase the 'totalSupply' by "_value".
      2.Increase the balance of the "_address" by "_value".

4. As mentioned in the assessment, the contract should have a 'burn' function that decreases the total supply and the balance of the "sender" address by a given value. It would work opposite to the mint functiion but will have the same parameters: 
   1. Parameters:
        1. _address: The address from which the tokens will be burned.
        2._value: The amount of tokens to be burned.
   2. The following actions will be performed once the burn function is called:
       1. Check if the balance of the _address is greater than or equal to _value.
       2. If true, decrease the totalSupply by _value.
       3. Decrease the balance of the `_address` by `_value`.
5. As per the requirements mentioned in the assessment ,the contact requires conditionals that will make sure the balance of the account is greater than or equal to the amount that is supposed to be burned .
This action would be achieved through the if statement If the conditional statement results to be false then nothing will happen. 
## COMPILATION AND DEPLOYMENT OF THE SMART CONTRACT: 

1. Deploy the 'Ethbeginner' contract to a supported Ethereum network. Here we used the Remix ID. 

2. Once deployed, you can interact with the contract by calling the following functions:

   1.Mint Function : Creates new tokens and assigns them to a specified address.
     
   2.Burn Function : Destroys existing tokens by reducing the total supply and the balance of a specified address.
    
