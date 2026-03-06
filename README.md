# Personal Expense Tracker

A command-line based personal expense and budget tracking application built in Java. This tool allows users to log their expenses, categorize them, set budgets, and gain insights into their spending habits.

## Features

-   **User Authentication**: Secure login for user-specific data.
-   **Expense Tracking**: Record both digital (bank-related) and physical (cash) expenses.
-   **Budget Management**: Create budgets for specific time periods, with the option to link them to expense categories.
-   **Categorization**: Organize expenses into user-defined categories.
-   **Bank Account Management**: Add and associate digital bank accounts with your user profile.
-   **Reporting & Insights**:
    -   View expenses summarized by day, month, or category.
    -   Calculate total expenses and remaining budget.
    -   Get insights like the daily average expense for a month and the percentage of total spending per category.

## Core Classes

The application is structured around several key classes:

-   `ExpenseTracker.java`: The main class that drives the application. It contains the CLI menu, manages lists of expenses and budgets, and holds the `main` method.
-   `User.java`: Represents the user, storing their profile information, credentials, and a list of associated `Bank` accounts.
-   `Expense.java`: Models a single expense transaction. It includes details such as amount, date, currency, and an optional category and bank information. Expense IDs are generated automatically.
-   `Budget.java`: Represents a budget with a specified amount, start date, end date, and an optional category. Budget IDs are also generated automatically.
-   `Bank.java`: A simple data class to hold a bank's name and account number.
-   `DateTime.java`: A helper class for managing date and time information for expenses and budgets.


## Usage

After a successful login, you will be presented with the main menu.

```
[1] Add Digital Bank
[2] Add New Expense
[3] Add New Budget
[4] Add Category
[5] View Expenses/Budgets
[6] View Insights
[7] View Remaining Budget
[8] Quit
Enter your choice:
```

-   **Add Digital Bank**: Add a new bank name and account number to your profile.
-   **Add New Expense**: Record a new expense, specifying if it's digital or physical and assigning an optional category.
-   **Add New Budget**: Create a new budget for a given time frame, with an optional category.
-   **Add Category**: Define a new category for organizing your expenses.
-   **View Expenses/Budgets**: Access sub-menus to view expenses by day, month, category, or view all at once.
-   **View Insights**: Analyze your spending with metrics like daily average or category percentages.
-   **View Remaining Budget**: Check the remaining amount in a specific budget after accounting for relevant expenses.
-   **Quit**: Log out and exit the application.
