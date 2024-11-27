Expense Tracker App
This is a simple Expense Tracker application built with React and Context API. It allows users to track their income and expenses, view their balance, and add or delete transactions in real time.

Features
View total balance.
Add income or expense transactions.
Display transaction history.
Delete transactions.
Simple UI with categorized income and expense display.
Tech Stack
Frontend: React
State Management: Context API, useReducer
Styling: CSS
Installation
1. Clone the repository:
bash
Copy code
git clone https://github.com/your-username/expense-tracker-app.git
cd expense-tracker-app
2. Install dependencies:
bash
Copy code
npm install
3. Start the application:
bash
Copy code
npm start
The app will be available at http://localhost:3000.

Project Structure
java
Copy code
├── src
│   ├── components
│   │   ├── AddTransaction.js
│   │   ├── Balance.js
│   │   ├── IncomeExpenses.js
│   │   ├── Transaction.js
│   │   └── TransactionList.js
│   ├── context
│   │   ├── GlobalState.js
│   │   └── AppReducer.js
│   └── App.js
├── public
├── package.json
└── README.md
Components Overview
1. Balance Component
Displays the user's total balance by summing all transactions.

2. IncomeExpenses Component
Displays total income and total expenses separately.

3. TransactionList Component
Shows a list of all transactions and provides a delete button for each.

4. AddTransaction Component
Allows users to add new transactions with a description and amount (positive for income, negative for expenses).

5. Transaction Component
Represents an individual transaction entry with delete functionality.

Context API & State Management
The app uses React's Context API and useReducer for global state management. Transactions are managed through actions:

ADD_TRANSACTION: Adds a new transaction.
DELETE_TRANSACTION: Removes a transaction by ID.
How to Use
Add a Transaction: Enter a description and amount. Positive amounts represent income; negative amounts represent expenses.
View Balance: The balance updates automatically as transactions are added or deleted.
Delete Transactions: Click the "x" button to remove a transaction.
Future Enhancements
Persist transactions in local storage or a database.
Add categories for transactions.
Enhance UI with animations or charts.
Implement authentication.
