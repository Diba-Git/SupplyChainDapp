# ACL Design Pattern

## Building out AccessControl Contracts
In this requirement, the barberryaccesscontrol contracts have been built out (FarmerRole.sol, DistributorRole.sol, RetailerRole.sol, and ConsumerRole.sol).

## Building out Base Contract
In this requirement, the barberrybase Contract (SupplyChain.sol) is built out. It is noteworthy that the ownership management in this contract is not used, and the one in the Core Contract (ownable.sol) is used instead.

## Building out Core Contract
This requirement has already been provided in the starter code that this project intends to build on. the barberrycore Contract, the ownership management used is the one in this contract.

## Defining and implementing inheritance
The first requirement of the second step of this project focuses on the inheritance structure of the smart contracts. This has been established like this:
•	The contracts FarmerRole, DistributorRole, RetailerRole, and ConsumerRole, import the library Roles. In this way, they can access functionality provided by (they inherit from) Roles.
•	The contract SupplyChain inherits from FarmerRole, DistributorRole, RetailerRole, and ConsumerRole. That means that all functionality within the Role contracts can be used within (is inherited by) SupplyChain.
•	The contract SupplyChain inherits from Ownable. In other words, all functionality within the Ownable contract can be used within (is inherited by) SupplyChain.
