# Brain Email Sorter

![Brain Logo](logo.png)

**Brain Email Sort** is a standalone email sorting tool that organizes email addresses by their MX (Mail Exchange) provider and detects cPanel webmail availability.

## 🚀 Features

- **MX Provider Detection**: Automatically identifies email providers (Gmail, Outlook, Yahoo, etc.)
- **cPanel Webmail Detection**: Detects domains with cPanel webmail access
- **Multi-threaded Processing**: Fast concurrent email processing
- **Easy Export**: Save sorted results by provider
- **Clean UI**: Modern dark-themed interface

## 📋 Requirements

- Python 3.8+
- Windows/Linux/macOS

## 🛠️ Installation

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Run the application:

```bash
python Brain_Email_Sort.py
```

## 🎯 Usage

1. **Load Email List**: Click "Browse" to select a text file with emails (one per line)
2. **Configure Options**:
   - Enable/disable MX provider sorting
   - Enable/disable cPanel webmail detection
   - Set number of threads (1-50)
3. **Start Sorting**: Click "Start Sorting" to process emails
4. **Export Results**: Save sorted emails to separate files by provider

## 📊 Supported Providers

- Gmail
- Outlook/Hotmail
- Yahoo
- AOL
- iCloud
- Zoho
- GoDaddy
- Amazon SES
- Rackspace
- Namecheap
- QQ Mail
- Yandex
- Mailgun
- NetEase (163.com)
- Other custom domains

## 🌐 cPanel Webmail Detection

The tool detects cPanel webmail by checking:

- Port 2095 (HTTP webmail)
- Port 2096 (HTTPS webmail)
- Common webmail paths (/webmail, /cpanel)
- Webmail subdomains (webmail.domain.com, mail.domain.com)

Public email providers (Gmail, Outlook, etc.) are automatically excluded from webmail detection.

## 💾 Output Format

Results are exported as text files:

- `gmail.txt` - All Gmail addresses
- `outlook.txt` - All Outlook addresses
- `cpanel_webmail.txt` - Emails with cPanel webmail detected
- ... (one file per provider)

## ⚙️ Performance

- Default: 10 threads
- Recommended: 10-20 threads for optimal performance
- Higher threads = faster processing but more resource usage

## 📄 License

Part of the Brain Tools suite by Brain Lead.

## 🆘 Support

- **Telegram**: [@iampopg](https://t.me/iampopg)

---

**Brain Email Sort** - Intelligent Email Organization Tool
