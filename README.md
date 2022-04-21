# Ballot-Contract

**Voting from the solidity documentation
The following contract is quite complex, 
but showcases a lot of Solidity’s features. It implements a voting contract.
Of course, the main problems of electronic voting is how to assign voting rights to the correct persons and how to prevent manipulation.
We will not solve all problems here,
but at least we will show how delegated voting can be done so that vote counting is automatic and completely transparent at the same time.**


In this contract, I tried to Solve the Ballot contract by adding Time-events
i.e Limiting the voting contract to **5 Minutes**
and in some way adding a cool feature to the voting Ballot as seen in the solidity smart contract example

# What I Did?
I limited the voting period of each Ballot contract to 5 minutes.

# To do so, I implement the following by:
1. Adding a state variable startTime to record the voting start time.
2. Creating a modifier voteEnded that will check if the voting period is over.
3. Using that modifier in the **vote** function to forbid voting and revert the transaction after the deadline.
 
