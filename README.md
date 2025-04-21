# Automate-Finances

A Streamlit-based dashboard application for automating financial transaction categorization and visualization.

## Description

Automate-Finances is a simple yet powerful tool that helps you gain insights into your spending habits by automating the categorization of your financial transactions. Built with Streamlit, this app allows you to upload transaction CSV files from your bank, intelligently categorize expenses, and visualize your spending patterns through interactive charts.

## Features

- **CSV Upload**: Import transaction data directly from your bank exports
- **Intelligent Categorization**: Automatically categorize transactions based on keywords
- **Machine Learning**: The app learns from your categorizations to improve accuracy over time
- **Custom Categories**: Create and manage your own spending categories
- **Interactive Visualization**: See your spending breakdown with Plotly charts
- **Expense Tracking**: Focus on where your money is going with detailed expense analysis
- **Dual-Mode View**: Separate tabs for expenses (debits) and income (credits)
- **Persistent Settings**: Categories and keywords are saved between sessions

## Installation

1. Clone the repository:
```bash
git clone https://github.com/codingaslu/Automate-Finances.git
cd Automate-Finances
```

2. Install required dependencies:
```bash
pip install streamlit pandas plotly
```

## Usage

1. Start the application:
```bash
streamlit run app.py
```

2. Upload your transaction CSV file
   - Ensure your CSV has columns for Date, Details, Amount, and Debit/Credit

3. Manage your expense categories
   - Add new categories with the text input field
   - The app will remember transaction descriptions for future automatic categorization

4. Analyze your spending
   - View the expense breakdown in pie charts
   - See category totals in the summary table

## CSV Format Requirements

Your bank transaction CSV should include these columns:
- `Date`: Transaction date (format: DD MMM YYYY)
- `Details`: Transaction description/merchant name
- `Amount`: Transaction amount
- `Debit/Credit`: Indicator for expense (Debit) or income (Credit)

## How It Works

1. **Upload**: The app reads your CSV file and processes the transactions
2. **Categorization**: Transactions are automatically matched against known keywords
3. **Customization**: You can manually edit categories and add new ones
4. **Learning**: When you apply changes, the app remembers your categorizations
5. **Visualization**: Your spending is broken down into easy-to-understand charts

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
