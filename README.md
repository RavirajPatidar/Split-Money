# Splitwise Clone - Expense Sharing App

A simplified expense sharing application inspired by Splitwise, developed as part of a machine coding and backend design assignment.

## ✨ Features

### User Management
- Create users
- Track individual balances
- View how much a user owes or is owed

### Group Management
- Create groups
- Add users to groups
- Track group-level balances

### Expense Management
Supports multiple split strategies:
- **Equal split** - Divide expenses equally among participants
- **Exact amount split** - Custom amounts per user
- **Percentage split** - Split based on percentage contributions

Each expense records:
- Payer
- Total amount
- Split details per user

### Balance Tracking
- Tracks who owes whom
- Maintains user-level and group-level balances
- Avoids redundant or circular transactions

### Balance Simplification (Settlement)
- Calculates net balance per user
- Separates users into **debtors** and **creditors**
- Uses **greedy algorithm** to minimize transactions

## Settlement Logic

1. **Calculate net balance** for each user:
   - Positive balance = user should **receive** money (creditor)
   - Negative balance = user **owes** money (debtor)

2. **Separate users** into debtors and creditors lists

3. **Match debtors with creditors** using greedy approach until all balances are settled

## 🛠️ Technology Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **JavaScript** - Programming language
- **In-memory storage** - Data persistence

### Frontend
- **React** - UI library
- **Tailwind CSS** - Utility-first CSS framework
- **Vite** - Build tool & dev server

## 🚀 Quick Start

