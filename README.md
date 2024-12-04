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
It iterates through all of the accounts to find the account number of the account to be removed and assigns it to accountToRemoved.
Then it checks to make sure that the accountToRemove isn't null, and it removes it.
