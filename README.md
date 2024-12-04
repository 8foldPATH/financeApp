This project is a banking app which allows users to create an account, log in to view their account, transfer money between current and savings accounts, and send money to an account associated with another unique user.

The class structure is defined as below. A bank has a user, a user has an account, an account can be either a current account or a savings account, and an account has transactions.

![image](https://github.com/user-attachments/assets/a563c8de-7c99-4d0d-8153-844f893b5082)

Bank Class

The bank class is used to add accounts, remove accounts, and transfer money between accounts. 

It makes a list of accounts.

The functions are AddAccount, RemoveAccount, GetAccount, and Transfer.

AddAccount simply creates a new account, taking the account number to be created as an argument.

RemoveAccount takes the account number of the desired account to be removed as an argument. 
It then initialises the account to be removed with a null value.
It loops through all of the accounts to find the account number of the account to be removed and assigns it to accountToRemoved.
Then it checks to make sure that the accountToRemove isn't null, and it removes it.

GetAccount takes the account number of the desired account as an argument.
It loops through all of the accounts, and finds the account with the associated account number.
If it's found, it returns the account. If it cannot be found, it returns null.

Transfer takes three arguments: the account number of the account money is being sent from, the account number of the account money is being sent to, and the amount of money being sent.
The variable fromAccount calls GetAccount with fromAccountNumber as an argument.
The variable toAccount calls GetAccount with toAccountNumber as an argument.
It checks if the values for either of the accounts are null, and returns false if either is.
Then it checks if the balance in fromAccount is less than the amount, and returns false if it is.
If fromAccount and toAccount are returned, and if the balance in the fromAccount is equal to or greater than the amount, the amount is withdrawn from fromAccount and the same amount is deposited in toAccount.
It then adds a transaction to the fromAccount and another one to the toAccount, and returns true.

