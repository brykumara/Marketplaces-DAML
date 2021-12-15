# Marketplaces-DAML
This is a submission I made for the individual coursework of COMP0163 Blockchain Technologies at UCL during the first half of my master's degree in November 2021. \
The task was to build a smart contract template on DAML for decentralized marketplaces. The following was requested:
1. Create a new contract template called Itemtosell that the seller can use to advertise a certain object and transfer ownership to a buyer . 
2. Add an insurer that can only view the information about the trade (without being able to issue or modify the contract Itemtosell).
3. In the contract you must specify the following: - Seller - Owner - Insurer - Type of item - Quantity - Price - Currency - Country.
4. Then, define the roles of the parties.
5. Add conditions to make sure that (i) the quantity and (ii) the price are larger than zero.
6. Add a function ChangePrice to modify the price listed in the contract where the controller is the “owner” of the item.
7. Add a function Sell that modifies the owner of the item listed in the contract where the controller is the “owner” of the item.

In the scenario testing part, using the following structure
``` setup = scenario do
-- Add parties
--Create contract
-- Trasnfer ownership
return()
you must:
1. Create three parties: “Party 1” (the seller), “Party 2” (the buyer), “Party 3” (the insurer).
2. Let the seller “Party 1” issue a new contract where the seller “Party 1” wishes to sell 1 watch for 100 GBP to “Party 2”. At this stage set the owner = the seller
3. Let the owner (=seller) of the watch transfer the ownership to “Party 2” (the buyer).
4. Describe one example where the execution of the contract would fail automatically and explain why this would happen.
