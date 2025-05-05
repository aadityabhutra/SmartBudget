# Smart Budget

## Overview
Smart Budget is an intelligent expense tracking and budgeting application built with Streamlit that helps users manage their personal finances effectively. The application leverages machine learning to automatically categorize expenses based on descriptions, provides comprehensive spending analysis with interactive visualizations, and alerts users when they exceed their predefined budget limits.


## Features

- **Expense Tracking**: Easily log your daily expenses with descriptions and amounts
- **Automated Categorization**: Uses machine learning (Multinomial Naive Bayes with TF-IDF) to predict expense categories based on descriptions
- **Interactive Dashboard**: View your spending patterns through intuitive pie charts and bar graphs
- **Budget Limits**: Set personalized spending limits for different expense categories
- **Email Alerts**: Receive email notifications when you exceed your daily spending limits
- **Daily Spending Analysis**: Track and visualize your daily expenditures by category
- **User-Friendly Interface**: Clean and intuitive design for a seamless experience

## Tech Stack

- **Frontend & Backend**: Streamlit
- **Data Processing**: Pandas, NumPy
- **Machine Learning**: Scikit-learn (TF-IDF Vectorizer, Multinomial Naive Bayes)
- **Data Visualization**: Matplotlib
- **Notifications**: SMTP email integration

## Installation

### Prerequisites
- Python 3.7+
- pip (Python package installer)

### Steps

1. Clone the repository
```bash
git clone https://github.com/your-username/smart-budget.git
cd smart-budget
```

2. Install required packages
```bash
pip install -r requirements.txt
```

3. Run the model training script (if not already trained)
```bash
python train_model.py
```

4. Launch the Streamlit app
```bash
streamlit run app.py
```

5. Access the app in your web browser at `http://localhost:8501`

## Usage Guide

### Adding Expenses
1. Enter the expense description (e.g., "Grocery shopping at Supermarket")
2. Input the amount spent
3. Click "Add Expense" to log the transaction
4. The app will automatically categorize your expense based on the description

### Setting Budget Limits
1. Navigate to the "Set Spending Limits" section
2. Enter your desired spending limit for each category
3. Limits will be used to monitor and alert you about overspending

### Email Notifications
1. Enter your email address and sender credentials in the "Check Limits and Send Email" section
2. Click "Check Limits and Send Email if Exceeded" to receive alerts when you've gone over budget
3. For security, consider using app-specific passwords for email services like Gmail

### Viewing Spending Analysis
- The app automatically generates pie charts and bar graphs to help you visualize spending patterns
- Daily analysis shows how you're spending your money across different categories

## Security Note
This application requires email credentials for sending alerts. We recommend using app-specific passwords instead of your main password. The app does not store these credentials beyond the current session.

## Future Enhancements
- Monthly and yearly spending analysis
- Export reports to PDF or Excel
- Multiple currency support
- Budget forecasting based on historical data
- Mobile app integration

## Contributing
Contributions to Smart Budget are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Thanks to all contributors who have helped shape Smart Budget
- Special thanks to the Streamlit team for making web app development with Python so accessible
