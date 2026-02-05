# SwiftCart

> A modern, high-performance auto-checkout solution with an intuitive desktop interface

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PyQt5](https://img.shields.io/badge/GUI-PyQt5-orange.svg)](https://www.riverbankcomputing.com/software/pyqt/)

SwiftCart is a professional auto-checkout application designed for rapid, automated purchasing workflows. Built with PyQt5, it provides a clean, modern interface for managing checkout tasks across multiple e-commerce platforms.

## ✨ Features

- **Multi-Platform Support**: Currently supports Walmart and Best Buy, with extensible architecture for additional retailers
- **Modern Desktop Interface**: Intuitive PyQt5-based GUI with dark theme and responsive design
- **Intelligent Monitoring**: Automatic restock detection with configurable monitoring intervals
- **Price Management**: Optional price checking and maximum price limits
- **Profile Management**: Secure storage and management of checkout profiles
- **Proxy Support**: Built-in proxy rotation for enhanced reliability
- **Webhook Integration**: Discord webhook notifications for order status updates
- **Fast Checkout**: Optimized checkout process for minimal latency

## 🚀 Quick Start

### Prerequisites

- Python 3.7 or higher
- Chrome browser (for Selenium automation)
- Internet connection

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/swiftcart.git
   cd swiftcart
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python app.py
   ```

## 📖 Usage

1. **Configure Profiles**: Navigate to the Profiles section and add your checkout information
2. **Set Up Proxies** (Optional): Add proxy lists in the Proxies section for enhanced reliability
3. **Create Tasks**: Use the Home page to create new checkout tasks with your desired settings
4. **Monitor & Execute**: The application will automatically monitor product availability and execute checkout when conditions are met

## 🏗️ Project Structure

```
swiftcart/
├── app.py                 # Main application entry point
├── settings.py            # Global application settings
├── utils.py               # Utility functions and helpers
├── webhook.py             # Discord webhook integration
├── requirements.txt       # Python dependencies
├── data/                  # Application data storage
│   ├── profiles.json      # User profiles
│   ├── proxies.json       # Proxy configurations
│   ├── settings.json      # User settings
│   └── tasks.json         # Task definitions
├── pages/                 # UI page components
│   ├── homepage.py        # Main dashboard
│   ├── createdialog.py    # Task creation dialog
│   ├── profilespage.py    # Profile management
│   ├── proxiespage.py     # Proxy management
│   └── settingspage.py    # Application settings
├── sites/                 # Retailer-specific implementations
│   ├── walmart.py         # Walmart checkout logic
│   ├── walmart_encryption.py  # Walmart encryption utilities
│   └── bestbuy.py         # Best Buy checkout logic
└── images/                # Application assets
    └── birdbot.png        # Application icon
```

## ⚙️ Configuration

Application settings can be configured through the Settings page in the GUI, or by directly editing `data/settings.json`. Key configuration options include:

- Webhook URL and notification preferences
- Browser behavior on failed checkouts
- Default monitoring and error delays

## 🔒 Security

- Profile data is encrypted using AES encryption
- Sensitive information is stored securely in JSON format
- Proxy credentials are handled securely

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Support

For support and questions, please open an issue on GitHub.

---

**Note**: This software is provided for educational purposes. Ensure compliance with retailer terms of service and applicable laws when using automated checkout tools.
