# Personal Finance Tracker

A comprehensive web application for tracking personal finances, enabling users to monitor and analyze their income and expenses with advanced categorization, filtering, and visualization features.

![Finance Tracker](https://img.shields.io/badge/React-18.x-blue) ![Status](https://img.shields.io/badge/Status-Complete-success)

## 🌟 Features

### Core Functionality
- ✅ **Transaction Management**: Add, edit, and delete income and expense transactions
- ✅ **Custom Categories**: Create and manage personalized income and expense categories
- ✅ **Advanced Filtering**: Filter transactions by type, category, and date range
- ✅ **Flexible Sorting**: Sort by date (newest/oldest) or amount (high-low/low-high)
- ✅ **Data Persistence**: All data saved locally using browser localStorage

### Enhanced Features
- 📊 **Visual Analytics**: 
  - Line chart showing income vs expenses over time
  - Pie chart displaying expense distribution by category
- 💾 **CSV Export**: Export filtered transactions for external analysis
- 📱 **Responsive Design**: Fully optimized for mobile, tablet, and desktop
- 🎨 **Modern UI**: Sleek gradient design with intuitive user experience

### Dashboard Statistics
- Real-time calculation of total income
- Real-time calculation of total expenses
- Current balance (income - expenses)
- Color-coded visual indicators

## 🚀 Live Demo

**Deployed Application**: [View Live Demo](#) *(Add your deployed URL here)*

## 📋 Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager
- Modern web browser with localStorage support

## 🛠️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/Chidubemkingsley/personal_finance_tracker.git
cd personal_finance_tracker
```

2. **Install dependencies**
```bash
npm install
```

3. **Start the development server**
```bash
npm start
```

4. **Open your browser**
Navigate to `http://localhost:3000`

## 📦 Dependencies

```json
{
  "react": "^18.2.0",
  "react-dom": "^18.2.0",
  "recharts": "^2.5.0",
  "lucide-react": "^0.263.1",
  "tailwindcss": "^3.3.0"
}
```

## 💻 Technology Stack

- **Frontend Framework**: React.js (with Hooks)
- **Styling**: Tailwind CSS
- **Charts**: Recharts library
- **Icons**: Lucide React
- **Data Storage**: Browser localStorage API
- **Build Tool**: Create React App / Vite

## 📖 How to Use

### Adding a Transaction

1. Click the **"Add Transaction"** button
2. Select transaction type (Income or Expense)
3. Enter the amount
4. Choose a date
5. Select a category
6. Add optional notes
7. Click **"Add"** to save

### Managing Categories

1. Click **"Manage Categories"**
2. View existing income and expense categories
3. Add new categories by:
   - Selecting type (Income/Expense)
   - Entering category name
   - Clicking **"Add"**
4. Delete categories using the trash icon

### Filtering Transactions

Use the filter section to:
- Filter by transaction type (All/Income/Expense)
- Filter by specific category
- Set date range (start and end dates)
- Sort by date or amount

### Exporting Data

1. Apply desired filters
2. Click **"Export CSV"**
3. CSV file downloads with filtered transactions

## 🏗️ Project Structure

```
personal-finance-tracker/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   └── FinanceTracker.jsx
│   ├── App.jsx
│   ├── index.js
│   └── styles/
│       └── index.css
├── package.json
├── README.md
└── .gitignore
```

## 🔧 Configuration

### localStorage Structure

Data is stored in localStorage under the key `financeData`:

```javascript
{
  "transactions": [
    {
      "id": "1699999999999",
      "type": "income",
      "amount": 5000,
      "date": "2024-11-10",
      "category": "Salary",
      "notes": "Monthly salary",
      "timestamp": "2024-11-10T12:00:00.000Z"
    }
  ],
  "categories": {
    "income": ["Salary", "Freelance", "Investment", "Other"],
    "expense": ["Food", "Transport", "Utilities", "Entertainment", "Healthcare", "Other"]
  }
}
```

## 🧪 Testing

### Manual Testing Checklist

- [ ] Add income transaction
- [ ] Add expense transaction
- [ ] Edit existing transaction
- [ ] Delete transaction
- [ ] Create custom category
- [ ] Delete category
- [ ] Filter by type
- [ ] Filter by category
- [ ] Filter by date range
- [ ] Sort transactions
- [ ] Export CSV
- [ ] Refresh page (verify data persistence)
- [ ] Test on mobile device
- [ ] Test on tablet device

### Running Tests (if implemented)

```bash
npm test
```

## 🌐 Deployment

### GitHub Pages

1. Install gh-pages:
```bash
npm install --save-dev gh-pages
```

2. Add to package.json:
```json
"homepage": "https://github.com/Chidubemkingsley/personal_finance_tracker.git",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

3. Deploy:
```bash
npm run deploy
```

### Vercel

1. Install Vercel CLI:
```bash
npm install -g vercel
```

2. Deploy:
```bash
vercel
```

### Netlify

1. Build the project:
```bash
npm run build
```

2. Drag and drop the `build` folder to Netlify

## 🎯 Technical Highlights

### State Management
- Uses React Hooks (useState, useEffect, useMemo)
- Efficient re-rendering with useMemo for calculations
- Centralized state management

### Performance Optimizations
- Memoized filtered transactions
- Memoized statistics calculations
- Memoized chart data
- Efficient array operations

### Responsive Design
- Mobile-first approach
- Tailwind CSS utility classes
- Flexible grid layouts
- Touch-friendly interface

## 📝 Git Workflow

This project follows best practices for Git workflow:

```bash
# Feature branches
git checkout -b feature/transaction-form
git checkout -b feature/charts
git checkout -b feature/csv-export

# Development branch
git checkout -b develop

# Pull requests
# Create PR from feature branches to develop
# Create PR from develop to main
```

## 🔒 Data Privacy

- All data stored locally in browser
- No server-side storage
- No personal data transmitted
- Data can be cleared via browser settings

## 🐛 Known Issues

- None at this time

## 🚀 Future Enhancements

- [ ] Multi-currency support
- [ ] Recurring transactions
- [ ] Budget planning features
- [ ] Data import from CSV
- [ ] Cloud backup integration
- [ ] Mobile app version
- [ ] Dark/Light theme toggle
- [ ] Transaction search functionality
- [ ] Email/SMS notifications
- [ ] Multi-user support

## 👨‍💻 Author

**Your Name**
- GitHub: [Chidubemkingsley](https://github.com/Chidubemkingsley/personal_finance_tracker.git)
- Email: kingsleycaesar581@gmail.com

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- React.js documentation
- Recharts library for charts
- Tailwind CSS for styling
- Lucide React for icons

## 📞 Support

For support, please open an issue in the GitHub repository or contact the author directly.

---

**Note**: This application was developed as part of a technical assessment demonstrating proficiency in:
- JavaScript/React.js
- State management
- Data persistence
- Responsive design
- Git workflow
- Modern UI/UX principles
