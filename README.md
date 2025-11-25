# 🚀 iRolixBot

<div align="center">

![iRolix Logo](iRolix%20Logo/iRolix%20Logo.png)

| [![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/iitzSeriZdev/iRolixBot) [![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE) [![PHP](https://img.shields.io/badge/PHP-8.2%2B-7777BB?logo=php)](https://php.net) ⚡ **Advanced Telegram VPN Sales Bot with Admin Panel**

**The Ultimate Solution for VPN Service Providers**

Transform your VPN business with a powerful, feature-rich Telegram bot that automates sales, manages users, and streamlines your operations.

[English](#) • [فارسی](README.fa.md) • [中文](README.zh.md) • [Русский](README.ru.md)

[🌟 Star](https://github.com/iitzSeriZdev/iRolixBot) • [🐛 Report Bug](https://t.me/iRolix_Bot/8) • [💡 Request Feature](https://t.me/iRolix_Bot/10) • [📖 Documentation](#-documentation)

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🎯 Key Highlights](#-key-highlights)
- [📦 Requirements](#-requirements)
- [🚀 Quick Start](#-quick-start)
- [⚙️ Configuration](#️-configuration)
- [🌐 VPN Panel Support](#-vpn-panel-support)
- [💳 Payment Gateways](#-payment-gateways)
- [🔒 Security](#-security)
- [📚 Documentation](#-documentation)
- [💬 Support & Community](#-support--community)
- [💰 Support Development](#-support-development)
- [📄 License](#-license)

---

## ✨ Features

### 🤖 Bot Features

- **📱 Subscription Management**
  - Purchase subscriptions (type, volume, duration)
  - Service renewal and extension
  - Extra volume and days purchase
  - Test service (one-time)
  - Service information and details

- **👥 User Management**
  - User account information
  - Transaction history
  - Referral statistics
  - Balance management

- **💳 Payment System**
  - Multiple payment gateways (Zarinpal, Card-to-Card, and more)
  - Automatic payment processing
  - Invoice management
  - Payment verification

- **🎁 Referral Program**
  - Unique referral links
  - Customizable commission (percentage/fixed)
  - Automatic payout
  - Referral statistics

- **🎫 Support System**
  - Ticket-based support
  - Admin notifications
  - Message forwarding

### 👨‍💼 Admin Features

- **📊 In-Bot Admin Panel**
  - User management
  - Service management
  - Product management
  - Panel management
  - Logs and statistics
  - Settings configuration

- **🌐 Web Admin Panel**
  - Complete dashboard with statistics
  - User management interface
  - Service management
  - Product management
  - VPN panel management
  - Invoice management
  - Referral system management
  - Security monitoring
  - Comprehensive logging
  - Multi-language support (English, Persian, Chinese, Russian)

### 🔒 Security Features

- **🛡️ Anti-Spam System**
  - Configurable click rate limits
  - Automatic mute functionality
  - Time-based restrictions

- **🚨 Anti-Fraud System**
  - Admin activity monitoring
  - Automatic access revocation
  - Suspicious activity detection

- **📊 Security Monitoring**
  - IP tracking
  - Browser and OS detection
  - Country detection
  - Activity logging

- **🔐 Additional Security**
  - Telegram IP verification
  - SQL injection prevention
  - XSS protection
  - CSRF protection
  - Rate limiting
  - Secure session management

---

## 🎯 Key Highlights

- ✅ **Multi-Language Support** - Full support for English, Persian, Chinese, and Russian
- ✅ **Dual Bot Architecture** - PHP bot for shared hosting, Python bot for VPS
- ✅ **Multiple VPN Panels** - Support for 12+ VPN panel types
- ✅ **Payment Gateways** - Integration with Iranian and international payment gateways
- ✅ **Automated Installation** - One-click installation for both hosting types
- ✅ **Professional Admin Panel** - Web-based admin panel with modern UI
- ✅ **Advanced Security** - Anti-spam, anti-fraud, and comprehensive monitoring
- ✅ **Referral System** - Complete referral and affiliate program
- ✅ **QR Code Generation** - Custom QR codes with background images

---

## 📦 Requirements

### Server Requirements

**For PHP Bot (Shared Hosting):**
- PHP >= 8.1
- MySQL/MariaDB >= 5.7
- Apache/Nginx with mod_rewrite
- cURL extension
- PDO MySQL extension
- mbstring extension
- GD extension (for QR codes)
- BCMath extension
- Write permissions for logs and uploads

**For Python Bot (VPS):**
- Python 3.9+
- MySQL/MariaDB >= 5.7
- Nginx (recommended)
- Systemd (for service management)

### PHP Extensions

- `pdo_mysql` - Database connection
- `curl` - HTTP requests
- `json` - JSON processing
- `mbstring` - Multibyte string handling
- `gd` - Image processing (QR codes)
- `bcmath` - Mathematical operations

### PHP Libraries (Composer)

- `endroid/qr-code` ^4.0 - QR code generation
- `guzzlehttp/guzzle` ^7.0 - HTTP client

---

## 🚀 Quick Start

### 📦 Automated Installation (Recommended)

#### For Shared Hosting

1. Upload all project files to your hosting
2. Navigate to: `https://yourdomain.com/installer/host/install.php`
3. Follow the installation wizard:
   - Step 1: Check requirements
   - Step 2: Configure database
   - Step 3: Configure bot
   - Step 4: Automatic installation
   - Step 5: Complete!

#### For VPS (Ubuntu/Debian)

```bash
# Install with one command
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) install

# Uninstall with backup
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) uninstall-with-backup

# Update directly
sudo bash <(curl -sSL https://raw.githubusercontent.com/iitzSeriZdev/iRolixBot/main/installer/vps/install.sh) update
```

**After installation:**

1. Database credentials are saved to `/tmp/irolix_db_config`
2. Edit `/opt/iRolixBot/bot-php/config.php` to add your bot token
3. Access the panel at `http://YOUR_SERVER_IP/web-panel`
4. Complete the setup through the web interface

### 📦 Manual Installation

If you prefer manual installation:

#### Step 1: Clone the Repository

```bash
git clone https://github.com/iitzSeriZdev/iRolixBot.git
cd iRolixBot
```

#### Step 2: Install Dependencies

```bash
cd bot-php
composer install
```

#### Step 3: Setup Database

Create a MySQL/MariaDB database and note the credentials.

#### Step 4: Create Telegram Bot

1. Message @BotFather on Telegram
2. Use `/newbot` to create your bot
3. Save the bot token securely

#### Step 5: Run Installation

1. Upload files to your web server
2. Visit `installer/host/install.php` in your browser
3. Follow the intuitive installation wizard:
   - Choose your language
   - Enter database details
   - Configure bot token
   - Set up admin account
   - Complete installation

#### Step 6: Setup Cron Jobs

Configure **just one cron job**:

```bash
* * * * * /usr/bin/php /path/to/iRolixBot/bot-php/cron/cron.php >> /path/to/iRolixBot/Logs/cron_output.log 2>&1
```

Or use HTTP:

```bash
* * * * * curl -s https://yourdomain.com/bot-php/cron/cron.php > /dev/null 2>&1
```

**That's it!** The centralized manager handles everything automatically. 🎉

---

## ⚙️ Configuration

After installation, customize your bot:

1. **🔌 VPN Panels** - Connect your panels
2. **💳 Payment Gateways** - Setup payment methods
3. **⚙️ Bot Settings** - Customize behavior
4. **👥 Users** - Manage customers
5. **🛍️ Products** - Create offerings
6. **📁 Categories** - Organize products

---

## ⏰ Cron Jobs

### What Gets Executed Automatically?

- **Every minute** ⚡ - Payments, notifications, messages
- **Every 2 minutes** 🎁 - Gift system, config testing
- **Every 3 minutes** 💰 - Payment gateway checks
- **Every 5 minutes** 📊 - Payment expiration, reports
- **Every 15 minutes** 🔍 - Status checks, monitoring
- **Every 30 minutes** ⏳ - Agent expiration
- **Every hour** 🎲 - Lottery system
- **Every 5 hours** 💾 - Automatic backups

---

## 🌐 VPN Panel Support

### OpexCore Library Panels:
- ✅ **Marzban** - Modern V2Ray/Xray panel
- ✅ **Marzneshin** - Advanced VPN panel
- ✅ **ovPanel** - OpenVPN panel
- ✅ **Pasarguard** - Secure VPN panel
- ✅ **Remnawave** - Wave VPN panel
- ✅ **Guard Panel** - Security-focused panel

### PHP-Based Panels:
- ✅ **Ali Reza** - Popular Iranian panel
- ✅ **Ali Reza Single Port** - Single port variant
- ✅ **3x-ui** - Xray UI panel
- ✅ **x-ui Single Port** - Single port Xray UI
- ✅ **S-ui** - Simple UI panel
- ✅ **Mikrotik** - RouterOS integration
- ✅ **WGDashboard** - WireGuard dashboard
- ✅ **Hiddify** - Hiddify panel
- ✅ **Sanaei** - Sanaei panel

---

## 💳 Payment Gateways

### Iranian Gateways:
- ✅ **Zarinpal** - Most popular Iranian gateway
- ✅ **Nowpayment** - Modern payment gateway
- ✅ **IranPay1** - Iranian payment gateway
- ✅ **Aqayepardakht** - Payment gateway
- ✅ **Card-to-Card** - Direct card transfer

### International Gateways:
- ✅ **Yoomoney** - Russian payment system
- ✅ **Yookassa** - Yandex payment gateway
- ✅ **Freekassa** - International gateway
- ✅ **Heleket** - Payment gateway
- ✅ **Robokassa** - Russian payment gateway
- ✅ **Telegram Stars** - Telegram's payment system
- ✅ **Cryptomus** - Cryptocurrency gateway
- ✅ **CryptoPay** - Crypto payment gateway

---

## 🔒 Security

### Security Features

- ✅ Telegram IP verification
- ✅ SQL injection prevention (Prepared Statements)
- ✅ XSS protection
- ✅ CSRF protection
- ✅ Rate limiting
- ✅ Secure session management
- ✅ Anti-spam system
- ✅ Anti-fraud system
- ✅ Security monitoring

### Security Best Practices

1. **After Installation:**
   - Delete the `installer` directory
   - Change default passwords
   - Set up SSL/TLS certificate

2. **Regular Maintenance:**
   - Update dependencies regularly
   - Review logs regularly
   - Backup database regularly

3. **Server Security:**
   - Use strong passwords
   - Enable firewall
   - Keep system updated

For detailed security information, see [SECURITY.md](SECURITY.md)

---

## 📚 Documentation

- 📖 [Installation Guide](HOST_INSTALLATION_GUIDE.md)
- 🔒 [Security Guide](SECURITY.md)
- ⏰ [Cron Setup](CRON_SETUP.md)
- 📊 [Project Summary](PROJECT_SUMMARY_FOR_HOST.md)

---

## 💬 Support & Community

### Get Help

- 💬 **Telegram Group**: [@iRolix_Bot](https://t.me/iRolix_Bot) - Join our community!
- 🐛 **Bug Reports**: [Report an Issue](https://t.me/iRolix_Bot/8) - Help us improve!
- 💡 **Suggestions**: [Share Ideas](https://t.me/iRolix_Bot/10) - Your ideas matter!

### Follow the Developer

- 🐙 **GitHub**: [@iitzSeriZdev](https://github.com/iitzSeriZdev)
- 🎥 **YouTube**: [@iitzSeriZ](https://youtube.com/@iitzSeriZ)
- 🐦 **X (Twitter)**: [@iitzSeriZ](https://x.com/iitzSeriZ)

---

## 💰 Support Development

### 🌟 Help Us Build the Future! 🌟

**Your support makes all the difference in the world!**

We're committed to making iRolixBot the best Telegram bot solution available. Your donations directly fuel faster development, exclusive features, and continuous improvements.

### 🚀 Why Your Donation Matters

Your generous donations enable us to:

- ⚡ **Accelerate Development** - More donations = faster feature releases and updates
- 🎯 **Build Exclusive Features** - Get access to cutting-edge capabilities
- 🛠️ **Enhanced Support** - Priority support for our generous donors
- 🌟 **Continuous Innovation** - Keep the project alive, thriving, and constantly evolving
- 🔒 **Better Security** - Invest in security audits and improvements
- 📚 **Comprehensive Documentation** - Create better guides and tutorials

### 💎 The More You Give, The More You Get!

**Every donation brings us closer to our goals!**

- **Higher donations** = **Priority access** to new features
- **Faster updates** = **More frequent releases** with bug fixes and improvements
- **Exclusive features** = **Unique capabilities** that set iRolixBot apart
- **Better support** = **Faster response times** and dedicated assistance

### 💳 How to Donate

Choose your preferred payment method:

#### 💰 Cryptocurrency (Direct Transfer)

| Currency    | Network                     | Address                                          |
| ----------- | --------------------------- | ------------------------------------------------ |
| 💵 **USDT** | BEP20 (Binance Smart Chain) | 0xCaF05b21A518E6750AA43aD87cEB4a725e78a850       |
| 💎 **TON**  | The Open Network            | UQAg7NaXzzFMvGxqirO9UYwwzseq8pAi3N8fompkKjOFtIzl |
| 💰 **TRX**  | Tron Network                | TPatJCKdLJs1ZpetLtpC97nsHg8X9G1KRs               |

> ⚠️ **Important:** Make sure you're using the correct network when sending cryptocurrency!

#### 💸 Online Payment (Recommended)

**🌐 Donate via NowPayments**

NowPayments accepts:
- 💳 Credit/Debit Cards
- 💰 100+ Cryptocurrencies
- 🌍 Multiple payment methods
- 🔒 Secure & Fast Processing

**Every donation, no matter the size, helps us improve iRolixBot and bring you better features!** 🙏

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

You're free to use, modify, and distribute this project! 🎉

---

<div align="center">

### Made with 💜 by iitzSeriZ

**Star this repo if you find it helpful!** ⭐

⭐ [Star](https://github.com/iitzSeriZdev/iRolixBot) • 🐛 [Report Bug](https://t.me/iRolix_Bot/8) • 💡 [Request Feature](https://t.me/iRolix_Bot/10) • 💸 [Donate](#-support-development)

**#woman_life_freedom**

</div>
