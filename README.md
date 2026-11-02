# Expenses-Analyser-CS-193-
Spending Tracker
A Java command-line tool that accepts my debit and credit transaction history as CSV exports, asks me to categorize each transaction, and generates weekly and monthly spending breakdowns against how much I received that month (from my job, from my parents, etc.).

The Problem:
I want to understand where my money goes each week, but bank statements show cryptic merchant names and don't tell me whether a purchase was groceries, a commute, or a "fun" non-essentials purchase.

How it works:
1. You download the CSV exports for your debit card and credit card from your bank.
2. You upload the CSV files to the program.
3. Finds how much you earned that week, and the program adds it to the balance file.
4. The program shows each transaction one at a time and asks you to categorize it. You pick from the existing categories. If none fit, you can add a new category.
5. As you categorize, the program deducts the amount from your balance information.
6. Once every transaction is categorized, the program generates the weekly analysis:
- Total money spent that week
- Percentage of the total spent in each category
- Whether you saved anything that week, and if so, how much
- If you saved money, the program deducts that amount from your debit account and adds it to your savings account.
7. If a budget is set, the program tells you how much you have left to spend in each category. Budgeting feature explained below.
8. The weekly analysis is saved in that month’s folder.

Budgeting:
Start of every month
- You review your categories and decide whether to add or remove any.
- You enter an estimated income for the month, since your income varies.
- You decide how much, or what percentage of income, to spend on each category.
- The program generates an estimated budget for each category from your estimate.

End of every month
- The program generates the monthly analysis and saves it in that month’s folder alongside the weekly ones.
- It tells you whether you stayed within budget in each category, and by how much you went over if you didn’t.
- When you enter your actual income for the month, the program reruns the analysis and budget comparison using that real number.

Files the program maintains
- A main file tracking your checking, savings, and loan (credit) account balances
- A folder for each month containing each week’s analysis and the full-month analysis. Created when you run the program.
