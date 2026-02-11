# Expense Tracker PWA 💰

A Progressive Web App (PWA) for tracking daily expenses and income. Built with HTML, CSS (Bootstrap), JavaScript (jQuery), and IndexedDB for local storage.

## ✨ Features

- 📱 **Installable**: Can be installed on Android, iOS, and desktop devices
- 🔌 **Offline Support**: Works completely offline after initial load
- 💾 **Local Storage**: All data stored locally using IndexedDB
- 📊 **Export to Excel**: Export transactions to Excel spreadsheet
- 🔍 **Filter Transactions**: Filter by account type
- 📅 **Date-based Organization**: Transactions organized by date
- 🎨 **Responsive Design**: Works on mobile, tablet, and desktop
- 🔄 **CRUD Operations**: Create, Read, Update, and Delete transactions

## 🚀 Live Demo

Visit the deployed app on GitHub Pages:
`https://[your-username].github.io/ExpenseTrackerPWA/`

## 📦 Installation

### On Android (Chrome)

1. Open the app in Chrome browser
2. Tap the menu icon (three dots) in the top right
3. Select **"Add to Home screen"** or **"Install app"**
4. Confirm by tapping **"Add"** or **"Install"**
5. The app will appear on your home screen like a native app

### On iOS (Safari)

1. Open the app in Safari browser
2. Tap the **Share** button (square with arrow pointing up)
3. Scroll down and tap **"Add to Home Screen"**
4. Enter a name (or keep "Expense Tracker")
5. Tap **"Add"**
6. The app will appear on your home screen

### On Desktop (Chrome/Edge)

1. Open the app in Chrome or Edge browser
2. Look for the install icon in the address bar (➕ or computer icon)
3. Click **"Install"**
4. The app will open in its own window

## 💻 Local Development

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server (optional, for testing)

### Running Locally

1. Clone this repository:
```bash
git clone https://github.com/[your-username]/ExpenseTrackerPWA.git
cd ExpenseTrackerPWA
```

2. Serve the files using a local web server:

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js:**
```bash
npx http-server
```

**Using PHP:**
```bash
php -S localhost:8000
```

3. Open your browser and navigate to:
```
http://localhost:8000
```

## 📁 File Structure

```
/
├── index.html              # Main application file
├── manifest.json           # PWA manifest configuration
├── service-worker.js       # Service worker for offline support
├── icons/
│   ├── icon-192x192.png    # App icon (192x192)
│   └── icon-512x512.png    # App icon (512x512)
└── README.md               # This file
```

## 🛠️ Technologies Used

- **HTML5**: Structure
- **CSS3**: Styling (via Bootstrap 5)
- **JavaScript**: Application logic
- **jQuery 3.6.0**: DOM manipulation
- **Bootstrap 5.0.2**: UI framework
- **SheetJS (xlsx)**: Excel export functionality
- **IndexedDB**: Local data storage
- **Service Workers**: Offline functionality
- **Web App Manifest**: PWA installation

## 📱 PWA Features

### Manifest

The `manifest.json` file defines:
- App name and short name
- Icons (192x192 and 512x512)
- Display mode (standalone)
- Theme color (#0d6efd - Bootstrap primary blue)
- Background color (#ffffff - white)
- Start URL

### Service Worker

The `service-worker.js` provides:
- **Cache-first strategy**: Loads from cache, falls back to network
- **Offline support**: App works without internet connection
- **Resource caching**: Caches all app assets and external libraries
- **Automatic updates**: Cleans up old caches on activation

## 🎯 Usage

### Adding a Transaction

1. Click **"Add Transaction"** button
2. Select the date
3. Choose the account (Bank, Expense, Salary, Box, Mom)
4. Select transaction type (From/To)
5. Enter description and amount
6. Add optional comments
7. Click **"Save"**

### Updating a Transaction

1. Click on any transaction in the list
2. Edit the details
3. Click **"Save"** to update or **"Delete"** to remove

### Filtering Transactions

- Click the **"All"** button to toggle between all transactions and Bank transactions only

### Exporting Data

- Click **"Export"** to download all transactions as an Excel file
- Data is organized by account type in separate sheets

### Clearing All Data

1. Click **"Clear Transactions"** button
2. Confirm the action
3. All transactions will be permanently deleted

## 🌐 Deployment on GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings**
3. Navigate to **Pages** in the left sidebar
4. Under **Source**, select the branch (usually `main`)
5. Click **Save**
6. Your app will be published at: `https://[your-username].github.io/ExpenseTrackerPWA/`

## 🔒 Privacy

- All data is stored locally in your browser's IndexedDB
- No data is sent to any server
- Your data stays completely private and on your device
- Clearing browser data will remove all transactions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 🐛 Known Issues

- Service worker caching may require manual refresh on updates
- iOS Safari has limited PWA support compared to Android Chrome

## 🔄 Future Enhancements

- [ ] Add categories for expenses
- [ ] Charts and visualizations
- [ ] Budget tracking
- [ ] Recurring transactions
- [ ] Multi-currency support
- [ ] Cloud backup option
- [ ] Dark mode

## 📞 Support

For issues or questions, please open an issue on GitHub.

---

Made with ❤️ for better expense tracking
