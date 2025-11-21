# Completed Project for Building Expense Tracker iOS App with Core Data & SwiftUI

![Alt text](./promo.png?raw=true "Building Expense Tracker iOS App with Core Data & SwiftUI")
Follow the tutorial at [alfianlosari.com](https://alfianlosari.com "Xcoding with Alfian Blog")

## Features

### Core Expense Management
* Create, edit, and delete expense logs
* Display list of expenses
* Filter expenses by categories and search query
* Sort expenses by date or amount in ascending or descending order
* Dashboard showing total expense sum for all and each category with pie chart visualization

### Group Expense Splitting
* Create groups with multiple members
* Split expenses equally or by custom amounts/percentages
* Track who paid and who owes what
* Automatic debt calculation and simplification
* View group balances and settle up debts

### Smart Features
* **Dashboard shows only YOUR split** - View only expenses you're responsible for
* **Clear Split** - Remove participants from an expense while keeping the expense record
* **Delete Expense** - Permanently delete expenses with automatic debt cleanup
* **Settled Splits Visualization** - See which splits are settled with green checkmarks (✓)
* **Filtered Debts** - View only debts involving YOU, not transactions between other members
* **Automatic Refresh** - All views update automatically when expenses are added, edited, or deleted

### User Experience
* Swipe actions for quick access to Clear Split and Delete options
* Context menu support for all actions
* Visual differentiation between settled and pending splits
* iOS 13.4+ compatibility with conditional UI features
* Real-time updates across Dashboard, Logs, and Groups tabs

## Requirements
- Xcode 11.4 or later
- iOS 13.4+

## Getting Started
- Clone or download the repository
- Open `ExpenseTracker.xcodeproj` in Xcode
- Build and Run (⌘R)

## Usage

### Managing Expenses
1. **Add Expense**: Tap "Add" button in Logs tab
2. **Edit Expense**: Tap on any expense or swipe left and tap "Edit"
3. **Delete Expense**: Swipe left on an expense and tap "Delete", or use the context menu
4. **Clear Split**: Swipe left on an expense with participants and tap "Clear Split"

### Group Expenses
1. **Create Group**: Go to Groups tab → Tap "Add" → Enter group name and select members
2. **Add Group Expense**: Open a group → Tap "+" → Fill expense details and select participants
3. **Split Options**:
   - **Equal**: Split amount equally among participants
   - **By Amount**: Specify custom amount for each participant
   - **By Percentage**: Specify percentage for each participant
4. **Settle Debts**: Go to "Show Balances" → Tap "Settle Up" on any debt

### Dashboard
- Shows only **YOUR split** amounts across all expenses
- Displays category-wise breakdown with pie chart
- Updates automatically when expenses change

## Recent Updates

### Version 2.0
- ✅ Added Clear Split and Delete Expense options to all views
- ✅ Dashboard now shows only YOUR split amounts
- ✅ Settled splits visualization with tick marks (✓)
- ✅ Filtered debts list to show only transactions involving YOU
- ✅ Automatic refresh across all views when expenses change
- ✅ Improved group expense management with debt tracking

## Project Structure
```
ExpenseTracker/
├── Models/
│   ├── ExpenseLog+Extension.swift
│   ├── ExpenseParticipant+Extension.swift
│   ├── Debt+Extension.swift
│   ├── Group+Extension.swift
│   ├── User+Extension.swift
│   └── CoreDataStack.swift
├── Views/
│   ├── Dashboard/
│   │   ├── DashboardTabView.swift
│   │   └── CategoryRowView.swift
│   ├── Logs/
│   │   ├── LogsTabView.swift
│   │   ├── LogListView.swift
│   │   └── LogFormView.swift
│   ├── Groups/
│   │   ├── GroupsTabView.swift
│   │   ├── GroupDetailView.swift
│   │   └── GroupFormView.swift
│   └── Common Views/
│       └── SwiftUICharts/
└── Helpers/
    └── Extensions.swift
```

## License
See LICENSE file for details
