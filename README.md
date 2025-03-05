def calculate_annual_expenses(expenses):
    """
    Calculate total annual expenses.
    :param expenses: Dictionary with categories as keys and monthly expenses as values.
    :return: Total annual expense.
    """
    total_annual = sum(expense * 12 for expense in expenses.values())
    return total_annual

# Example usage
monthly_expenses = {
    "Rent": 1200,
    "Utilities": 150,
    "Internet": 50,
    "Groceries": 400,
    "Transportation": 100,
    "Entertainment": 200
}

total = calculate_annual_expenses(monthly_expenses)
print(f"Total annual expenses: ${total}")
