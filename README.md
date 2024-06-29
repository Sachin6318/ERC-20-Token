# Create a ERC-20 token
This Solidity program is a simple smart contract to create your own"ERC20 token" and deploy it using Remix". It demonstrates the basic syntax and functionality of the ERC20 token in the Solidity programming language. The purpose of this program is to serve as a starting point for those who are new to "ERC20 token" in Solidity and want to get a feel for how it works.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. It is a simple smart contract to create your own "ERC20 token" and deploy it using Remix. This program serves as a simple and straightforward introduction to "ERC20 token" in Solidity programming, and can be used as a stepping stone for more complex projects in the future.

## Getting Started

Executing program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:



       
        // SPDX-License-Identifier: MIT
       // Compatible with OpenZeppelin Contracts ^5.0.0
          pragma solidity ^0.8.20;

        import "@openzeppelin/contracts@5.0.2/token/ERC20/ERC20.sol";
        import "@openzeppelin/contracts@5.0.2/token/ERC20/extensions/ERC20Burnable.sol";
        import "@openzeppelin/contracts@5.0.2/access/Ownable.sol";

       contract MyToken is ERC20, ERC20Burnable, Ownable {
           constructor(address initialOwner)
               ERC20("pikachu", "pika")
               Ownable(initialOwner)
           {}

           function mint(address to, uint256 amount) public onlyOwner {
               _mint(to, amount);
           }
       }

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.20" (or another compatible version), and then click on the "Compile" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar but first select the network to the testnet of "Avalanche Network" and connect your "Metmask" wallet. Once the contract is deployed, you can interact with it by calling mint, burn, transfer, balance functions.
## Authors

Sachin Singh

@Sachin17234

sachinsingh6318@gmail.com


## License

This project is licensed under the MIT License.
