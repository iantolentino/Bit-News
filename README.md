# 🚀 Bitcoin Trading Dashboard

A professional, responsive web application designed for Bitcoin traders that provides real-time market news, trading strategy guidance, and session timing alerts.

![Bitcoin Trading Dashboard](https://img.shields.io/badge/Bitcoin-Trading%20Dashboard-orange?style=for-the-badge)
![GitHub Pages](https://img.shields.io/badge/Deployed-GitHub%20Pages-blue?style=for-the-badge)
![Responsive](https://img.shields.io/badge/Design-Responsive-green?style=for-the-badge)

## ✨ Features

### 📰 Multi-Source News Aggregation
- **7 Free News APIs** integrated for comprehensive coverage
- Real-time Bitcoin and cryptocurrency news
- Automatic duplicate removal and smart sorting
- Sentiment analysis with color-coded indicators
- Maintains latest 20 news items with auto-refresh

### ⏰ Smart Trading Session Alerts
- **Philippines Time (PHT)** optimized schedule
- Dynamic status indicators for:
  - 🟢 **London Session** (4PM-7PM PHT) - High volatility
  - 🟡 **US Session** (9PM-12AM PHT) - Momentum moves
  - 🔴 **Asian Session** (8AM-12PM PHT) - Avoid trading
- Real-time clock and session status updates

### 📊 Trading Strategy Reference
- Clear entry/exit conditions
- RSI-based strategy with multi-timeframe confirmation
- Risk management rules
- Position sizing guidelines

### 🎨 Professional Design
- **Black & White** theme with **Red/Green** accents
- Fully responsive (mobile, tablet, desktop)
- Bootstrap 5 framework
- Clean, modern interface optimized for trading

## 🚀 Quick Start

### Option 1: Use Live Demo
Visit the deployed version: [Your GitHub Pages URL]

### Option 2: Deploy Your Own

1. **Fork this repository**
   ```bash
   git clone https://github.com/your-username/bitcoin-trading-dashboard.git
   ```

2. **Deploy to GitHub Pages**
   - Go to repository **Settings**
   - Scroll to **Pages** section
   - Select **main branch** as source
   - Your site will be live at: `https://your-username.github.io/bitcoin-trading-dashboard`

### Option 3: Local Development
```bash
# Clone the repository
git clone https://github.com/your-username/bitcoin-trading-dashboard.git

# Open in browser
cd bitcoin-trading-dashboard
open index.html
```

## 🛠️ Technical Details

### Built With
- **HTML5** - Semantic structure
- **CSS3** - Custom styling with CSS variables
- **Bootstrap 5** - Responsive framework
- **Vanilla JavaScript** - No dependencies required
- **GitHub Pages** - Free hosting

### News APIs Integrated
| API | Purpose | Status |
|-----|---------|---------|
| CryptoCompare | Crypto-specific news | ✅ Free |
| NewsAPI | General crypto news | ✅ Free |
| NewsData.io | Blockchain news | ✅ Free |
| CoinGecko | Market news | ✅ Free |
| Reddit r/CryptoCurrency | Community sentiment | ✅ Free |
| Reddit r/Bitcoin | Bitcoin discussions | ✅ Free |
| CryptoPanic | News aggregator | ✅ Free |

### File Structure
```
bitcoin-trading-dashboard/
├── index.html              # Main application file
├── assets/
│   └── bitcoin.png         # Favicon (add your own)
├── README.md              # This file
└── .gitignore            # Git ignore rules
```

## 💡 Trading Strategy

### Entry Conditions
- RSI ≤ 30 on 15-minute chart
- 5-min, 15-min & 1-hour bullish alignment
- EMA 20 > EMA 50 on all timeframes
- Green candle formation with volume increase

### Exit Conditions
- RSI reaches 65-80 range
- 0.5% profit target achieved
- Stop loss triggered at 0.3-0.4%

### Risk Management
- 0.3-0.4% risk per trade
- Maximum 2-5 trades per day
- $3 daily loss limit
- Position sizing based on signal quality

## 🕒 Optimal Trading Times (PHT)

| Session | Time (PHT) | Recommendation |
|---------|------------|----------------|
| **London Open** | 4:00 PM - 7:00 PM | 🟢 **ACTIVE** - High volatility |
| **US Open** | 9:00 PM - 12:00 AM | 🟡 **ACTIVE** - Momentum moves |
| **Asian Session** | 8:00 AM - 12:00 PM | 🔴 **AVOID** - Low liquidity |

**Best Trading Days:** Tuesday - Thursday

## 🔧 Configuration

### Customizing News Sources
Edit the `NEWS_APIS` array in the JavaScript section to:
- Add new APIs
- Modify existing endpoints
- Adjust refresh intervals

### Time Zone Adjustments
The dashboard uses Philippines Time (UTC+8). To modify:
```javascript
// In updateTimeAndStatus() function
const phTime = new Date(now.getTime() + (8 * 60 * 60 * 1000)); // Change UTC offset
```

### Styling Customization
CSS variables in the `<style>` section:
```css
:root {
    --black: #000000;
    --white: #ffffff;
    --red: #dc3545;
    --green: #198754;
    /* Modify these to change color scheme */
}
```

## 🐛 Troubleshooting

### Common Issues

**Favicon Not Displaying on GitHub Pages**
```html
<!-- Change from relative path -->
<link rel="icon" href="assets/bitcoin.png" type="image/x-icon" />

<!-- To absolute path or CDN -->
<link rel="icon" href="https://cdn.jsdelivr.net/gh/your-username/bitcoin-trading-dashboard/assets/bitcoin.png" type="image/x-icon" />
```

**News Not Loading**
- Check browser console for CORS errors
- Some APIs may have rate limits
- Try refreshing or waiting a few minutes

**Time Display Incorrect**
- Ensure JavaScript is enabled
- Check browser time zone settings

## 📈 Performance

- **Load Time:** ~2-3 seconds
- **News Refresh:** Every 10 minutes
- **Status Updates:** Every minute
- **API Success Rate:** 5-7/7 APIs typically functional

## 🤝 Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

### Development Guidelines
- Maintain black/white/red/green color scheme
- Ensure mobile responsiveness
- Test all API integrations
- Keep dependencies minimal

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

**Trading involves substantial risk of loss and is not suitable for every investor.** This dashboard is for educational and informational purposes only. The creators are not responsible for any trading decisions made based on the information provided.

- Past performance is not indicative of future results
- Always do your own research
- Never invest more than you can afford to lose
- Consider consulting with a qualified financial advisor

## 🆘 Support

If you encounter any issues:

1. Check the [Troubleshooting](#🐛-troubleshooting) section
2. Search existing [GitHub Issues](https://github.com/your-username/bitcoin-trading-dashboard/issues)
3. Create a new issue with details about the problem
