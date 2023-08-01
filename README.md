# Connecting frontend with the smart contract with metamask wallet.
Under this we are connecting our smart contract with frontend using metamask local host server.We are just creating a simple frontend and connect wallet and contract with it.

# Description
 I will explain my module on Solidity code. I will cover the license identifier, Solidity version, and the contract named "transactions." I will discuss the deposit function, which allows for receiving ether, and the withdrawal function, which transfers a specified amount.
 Additionally, I will explain the get balance function, which returns the balance of a given address, and the get address function, which returns the address where the transaction occurred. Finally, I will demonstrate how to compile and deploy the code using MetaMask and run it on the frontend we have created.
 
# Execution

//SPDX-License-Identifier: GPL-3.0
pragma solidity ^0.8.7;

contract Transactions {

    function deposit() external payable {
    }

    function withdraw(address payable _to, uint _amount) external {
        _to.transfer(_amount);
    }

    function getBalance() external view returns(uint) {
        return address(this).balance;
    }

    function getAddress() external view returns(address) {
        return address(this);
    }

}
Compile the code
We have to Deploy it using metamask environment on remix.Then we have to connect our metamask to frontend and after that we have to perform withdrawal and deposit functions.


# Authors

Dhruv Kalia.
