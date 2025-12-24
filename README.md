This project is a simplified expense sharing application inspired by Splitwise.
It was developed as part of a machine coding and backend design assignment.
The system allows users to create groups, add shared expenses using multiple split strategies, track balances, and simplify dues using settlement logic.
The primary focus is correctness of business logic, clean structure, and clarity of design decisions.

Features
User Management
  -Create users
  -Track individual balances
  -View how much a user owes or is owed
  
Group Management
  -Create users
  -Track individual balances
  -View how much a user owes or is owed

Expense Management
  -Supports the following split types
  -Equal split
  -Exact amount split
  -Percentage split

Each expense records:
  -Payer
  -Total amount
  -Split details per user

Balance Tracking
  -Tracks who owes whom
  -Maintains user-level balances
  -Avoids redundant or circular transactions

Balance Simplification (Settlement)
  -Calculates net balance per user
  -Separates users into debtors and creditors
  -Settles balances using a greedy approach to minimize transactions

Settlement Logic Explanation
  Calculate net balance for each user
    1)A positive balance indicates the user should receive money
    2)A negative balance indicates the user owes money
  Separate users into debtors and creditors
  Match debtors with creditors until all balances are settled


Technology Stack
Backend
  -Node.js
  -Express.js
  -JavaScript
  -In-memory data storage

Frontend
  -React
  -Tailwind CSS
  -Vite

  
