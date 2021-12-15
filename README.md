# Marketplaces-DAML


In this first exercise you have to build in a smart contract template in DAML that can be used for decentralized marketplaces. To do this, you are asked to create a new
contract template called Itemtosell that the seller can use to advertise a certain object and transfer ownership to a buyer . We also wish to add an insurer
that can only view the information about the trade (without being able to issue or modify the contract Itemtosell ).
Contract template
1. Start by creating a new project and .daml file.
2. Create a contract template called Itemtosell . [8 pts] In the contract you must specify the following:
- Seller - Owner - Insurer - Type of item - Quantity - Price - Currency - Country
3. Then, define the roles of the parties. What type of party should the seller be? And the insurer? [8 pts]
4. Add conditions to make sure that (i) the quantity and (ii) the price are larger than zero. [5 pts]
5. Add a function ChangePrice to modify the price listed in the contract where the controller is the “owner” of the item. [5 pts]
6. Add a function Sell that modifies the owner of the item listed in the contract where the controller is the “owner” of the item. [5 pts]
Scenario testing
In the scenario testing part, using the following structure
``` setup = scenario do
-- Add parties
--Create contract
-- Trasnfer ownership
return() ```
you must:
1. Create three parties: “Party 1” (the seller), “Party 2” (the buyer), “Party 3” (the insurer). [2 pts]
2. Let the seller “Party 1” issue a new contract where the seller “Party 1” wishes to sell 1 watch for 100 GBP to “Party 2”. At this stage set the owner = the seller [5
pts]
3. Let the owner (=seller) of the watch transfer the ownership to “Party 2” (the buyer). [5 pts]
4. Take a screenshot of the state of the ledger (by looking at the scenario results). [2 pts]
5. Describe one example where the execution of the contract would fail automatically and explain why this would happen. [5 pts]
