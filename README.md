# step3

Class Account

To create a bank account with some attributes

Attributes

account_id: account id.

balance: current balance of the account.

transaction_history: A list of all transactions by time.

password: The password for the account.

Methods

init(self, account_number, initial_balance, password)

Initializes a new account.

add_transaction(self, amount, transaction_type)

Records a new transaction.

update_balance(self, amount, transaction_type)

This method will upadate the account balance after transaction.

Class AccountControl

Manages banking accounts

Attributes

account: A dictionary storing all accounts, key is account id.

Methods

init(self)

Initializes the AccountControl

add_account(self, account)

Adds a new account to the our banking system.

check_balance(self, account_id)

check the balance based ob the account_id.

print_transaction_history(self, transactions)

print the transaction history in a good format

view_transaction_history(self, start_date=None, end_date=None)

retrun the transaction history for a user input date range.

execute_transaction(self, account_id, amount, transaction_type)

identify a transaction on a based account_id and transaction_type .

Class FinancialServices

financial services like fund transfer, deposit, and withdrawal.

Attributes

account_control: An instance of AccountControl.

Methods

init(self)

Initializes the FinancialServices instance.

fund_transfer(self, first_account_id, sec_account_id, amount)

Transfers funds between your accout or other's account.

deposit(self, user_id, amount) Deposits money into an account.

withdrawal(self, user_id, amount) Withdraws money from an account.

Class Authorize attibute: it inherite the Account class Methods: init(self, account_number, password, account_control): initialize the class.

login(self, entered_account_number, entered_password): It allows the users to log in their account when they have the valid set of account number and password which are in our database.

logout(self): It allows the users' current login status logged out.

delete_account(self, username) It allows the uers to delete their account once they are logged in.

Class CustomerService attribute: self(this is a class independent on the other 3 classes) init(self): method save_message(self) It allows users to write down their recommendation to our app and save it into our storage center.

customer_service(self): This can offer users the contact phone number and email address.

calculate_loan_repayment(self, loan_amount, loan_term, annual_interest_rate=0.05) The users can give this function loan_amount, period and interest rate as input, and this function will return the repayment as output. So it is similar to a calculator. 

https://pypi.org/project/zxyzhxbanking/0.1.0/
