# personalfinanceAPP

A simple command-line **Expense Tracker** written in Python. It lets you add daily expenses, list all saved expenses, and calculate total spending.

## Features

- Add an expense (date, category, description, amount)
- View all expenses entered in the current session
- View total spending ("Total Khrcha")
- Menu-driven CLI loop

## Project Files

- `index.py` — main program (runs the menu and stores expenses in memory)

## Requirements

- Python 3.x

## How to Run

```bash
python index.py
```

## How It Works

- Expenses are stored in a list called `expensesList` as dictionaries with keys: `date`, `category`, `description`, and `amount`.
- Data is stored **in memory only**; when you exit the program, expenses are lost.

## Menu Options

1. **Add Expense** — prompts for date, category (e.g., Food, Travel, Makeup, Books), description, and amount.
2. **View All Expenses** — prints each saved expense.
3. **View Total Khrcha** — sums the `amount` field of all saved expenses.
4. **Exit** — quits the program.

## Notes / Known Issues

- The current `index.py` has a small Python f-string quoting issue on the "View All Expenses" print line (nested double quotes). Using single quotes for dictionary keys inside the f-string will fix it (e.g., `eachKharcha['date']`).
