# BitcoinAnalytics
Bitcoin dataset from https://senseable2015-6.mit.edu/bitcoin/

# Transaction analysis
1. What is the number of transactions and addresses in the dataset?
2. What is the Bitcoin address that is holding the greatest amount of bitcoins? How much is that exactly? Note that the address here must bea valid Bitcoin address string. The balance here is the total amount of bitcoins in the UTXOs of an address.
3. What is the average balance per address?
4. What is the average number of input and output transactions per address? What is the average number of transactions per address.
5. What is the transaction that has the greatest number of inputs? How many inputs exactly? Show the hash of that transaction. If there are
multiple transactions that have the same greatest number of inputs, show all of them.
6. What is the average transaction value? Transaction value is the sum of all outputs’ value.
7. How many coinbase transactions are there in the dataset?
8. What is the average number of transactions per block?

# Address de-anonymization
In Bitcoin, a user may possess multiple addresses. In this part, a simple heuristic is applied to infer the Bitcoin users owning those addresses. 
The heuristic consists of two phases:
1. Joint control: assume that all input addresses of a transaction are controlled by the same user.  
2. Serial control: assume that the output address of a transaction with only a single output is controlled by the same user owning the input addresses.

This part answers the following questions
1. How many users are there in the dataset?
2. What is the Bitcoin user that is holding the greatest amount of bitcoins? How much is that exactly? 
3. What is the average balance per user?
4. What is the average number of input and output transactions per user? 
Note that each user is identified by the addresses that are owned by
them. 
5. Give the hash of the transaction sending the greatest number of bitcoins
to the user who is holding the greatest balance.
