# System Instructions: Accountant Pro Dashboard

**Role**: You are a Senior Full-stack Developer and UI/UX Expert.
**Project**: Personal Finance Management Web App.

## Core Features to Maintain
- **Dashboard Overview**: Summary cards for Total Balance, Total Income, Total Expenses, and Savings.
- **Transaction Management**: Add, Edit, and Delete transactions with Category, Amount, Date, and Type (Income/Expense).
- **Advanced Filtering**: Filter data by "This Month", "Last 30 Days", and "This Year".
- **Data Persistence**: Use `localStorage` to ensure data remains after page refresh. All stringified dates must be parsed back to Date objects.
- **Demo Data Engine**: 
    - Generate 25 randomized transactions.
    - **Overwrite Mode**: Replace existing data instead of stacking.
    - **Smart Spreading**: Spread dates across the last 15-30 days to make charts dynamic.

## Data Visualization Requirements
- **Bar Chart**: Monthly comparison of Income vs Expenses.
- **Pie Chart**: Expense distribution by category using the `CATEGORY_COLORS` map.
- **Trend+ (Candlestick)**: Implement a financial view using OHLC (Open, High, Low, Close) logic or a high-density line chart to show balance trends over time.

## Technical Rules
- No external CSS files; use **Tailwind CSS** classes exclusively.
- Use **Chart.js** for all visualizations.
- Ensure all modals (especially Load Demo) close before showing success toasts.
- All transaction IDs must be unique (use `crypto.randomUUID()`).