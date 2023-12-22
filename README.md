# MOD-3 Project
## About The Project 

*Mint, Burn & Transfer Token*
This is a Solidity smart contract for create your own ERC20 token and deploy it using HardHat or Remix. Once deployed, you should be able to interact with it for your walk-through video. From your chosen tool, the contract owner should be able to mint tokens to a provided address and any user should be able to burn and transfer tokens

## Introduction
In this Create a Contract To Mint The Token , Burn The Token and transfer the Token which is ERC20.

### Requirements
- Compiler Remix IDE or Hardhat
- pragma solidity 0.8.20
- Ethereum development Environment
- ERC20 and Ownable (Openzeppelin)


### Executing program
* Create a contract.
* Import the File Form openzeppelin library (ERC20 & Ownable)
* Function Mint
```
function mint(address account, uint256 amount) external onlyOwner {
        _mint(account, amount);
    }
```
This functions helps to Mint the Token to the Owner Address  next is

* Funtion Burn 

```
    function burn(uint256 amount) external onlyOwner {
    _burn(_msgSender(), amount);
}
```
the function to burn the token from the owner address by specified amount 

* Funtion TransferWithCheck 

```
 function transferWithCheck(address to, uint256 amount) external {

        _transfer(_msgSender(), to, amount);
    }
```
 The Transfer Function allow The Owner to Transfer the Token to Any Address by Specified Amount.

## Authors
PRATIK BELE

## License
This project is licensed under the [MIT] License - see the LICENSE.md file for details
