# Joint-Savings-Account

This Project aims on building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts. I will create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. This smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

## Methods and Techniques Used: 

The steps for this project are divided into the following sections:


### 1. Create a Joint Savings Account Contract in Solidity:

Here I will define a new contract named JointSavings. Then I will define two variables of type address payable named accountOne and accountTwo. Next I will make a new variable of type address public named lastToWithdraw. Next I will define two variables of type uint public named lastWithdrawAmount and contractBalance. Lastly I will define a function named withdraw that accepts two arguments: amount of type uint and recipient of type payable address. Next I will define a public payable function named deposit. Then I will define a public function named setAccounts that takes two address payable arguments, named account1 and account2. In the body of the function, I will set the values of accountOne and accountTwo to account1 and account2, respectively. Add a fallback function so that the contract can store ether that’s sent from outside the deposit function.

### 2. Compiling and Deploying My Contract in the JavaScript VM:

Next I will need to compile the smart contract.

In the Remix IDE, we will need to navigate to the “Deploy & Run Transactions” pane, and then make sure that “JavaScript VM” is selected as the environment.

Next we will click the Deploy button to deploy the smart contract, and then confirm that it successfully deployed.


### 3. Interacting with Deployed Smart Contract:

I will use the setAccounts function to define the authorized Ethereum address that will be able to withdraw funds from the contract.

Next I will test the deposit functionality of our smart contract by sending ether. After each transaction, I will use the contractBalance function to verify that the funds were added to my contract


Once I have successfully deposited funds into my contract, I will test the contract’s withdrawal functionality by withdrawing 5 ether into accountOne and 10 ether into accountTwo. After each transaction, I will need to use the contractBalance function to verify that the funds were withdrawn from your contract. Additionally I will use the lastToWithdraw and lastWithdrawAmount functions to verify that the address and amount were correct.

## Goal Of This Project:

The main goal of this project is to automate the creation of joint savings accounts be able to control a joint savings account. My smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.
