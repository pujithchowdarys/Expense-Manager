# Expense-Manager
Household Expense Manager
# Household Expense Manager

A web application for managing household expenses, business transactions, chits, and loans with Google Sheets integration.

## Features

- **Dashboard**: Overview of financial status with key metrics
- **Business Management**: Track customer transactions and balances
- **Chits Management**: Manage chit funds with lottery system
- **Household Expenses**: Track income and expenses by category
- **Loans Management**: Monitor loans taken and given
- **Summary Reports**: Visual charts and detailed financial summaries
- **Google Sheets Integration**: Sync all data with Google Sheets in real-time
- **Responsive Design**: Works on desktop, tablet, and mobile devices

## Live Demo

The application is hosted on GitHub Pages:
[https://your-username.github.io/repository-name](https://your-username.github.io/repository-name)

## Setup Instructions

### 1. Google Sheets Preparation

1. Create a copy of the template Google Sheet:
   [https://docs.google.com/spreadsheets/d/1ZQpgN7PU8kRhDnjIxOGJfY7IQkKRC3I1/edit](https://docs.google.com/spreadsheets/d/1ZQpgN7PU8kRhDnjIxOGJfY7IQkKRC3I1/edit)

2. Click "File" > "Make a copy" to create your own version

3. Note the Sheet ID from the URL (the long string between `/d/` and `/edit`)

### 2. Google Cloud Console Configuration

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)

2. Create a new project or select an existing one

3. Enable the Google Sheets API:
   - Navigate to "APIs & Services" > "Library"
   - Search for "Google Sheets API"
   - Click on it and press "Enable"

4. Create credentials:
   - Go to "APIs & Services" > "Credentials"
   - Click "Create Credentials" > "OAuth client ID"
   - Select "Web application" as the application type
   - Add authorized JavaScript origins:
     - `https://your-username.github.io`
   - Add authorized redirect URIs:
     - `https://your-username.github.io`
   - Click "Create" and note your Client ID

5. Create an API key:
   - Click "Create Credentials" > "API key"
   - Restrict the API key to only the Google Sheets API and your GitHub Pages domain

### 3. Application Configuration

1. Open the application on GitHub Pages

2. Navigate to the "Settings" tab

3. Enter your configuration:
   - Google Sheets URL: Your copied sheet URL
   - Google Client ID: Your OAuth 2.0 Client ID
   - Google Sheets API Key: Your generated API key
   - Select your preferred sync frequency

4. Click "Save Settings"

5. Click "Connect to Google Sheets" and authorize the application

## Usage

1. **Dashboard**: View your financial overview on the welcome page
2. **Business**: Add customers and track transactions
3. **Chits**: Manage chit funds and use the lottery system to select winners
4. **Expenses**: Add and categorize household income and expenses
5. **Loans**: Track loans taken and given with payment history
6. **Summary**: View detailed reports and charts of your finances
7. **Settings**: Configure Google Sheets integration

## Technical Details

- Built with HTML, CSS, and vanilla JavaScript
- Uses Google Sheets API for data storage
- Responsive design works on all devices
- Charts powered by Chart.js
- Icons from Font Awesome

## Privacy & Security

- All data is stored in your own Google Sheet
- The application only requests permissions to access your Google Sheets
- No data is stored on external servers

## Support

If you encounter any issues:
1. Ensure your Google Sheet has the required tabs
2. Verify your API keys and OAuth client ID are correctly configured
3. Check that your Google Sheet is shared with the service account

## License

This project is open source and available under the [MIT License](LICENSE).
