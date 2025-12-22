# 🚀 Bitcoin Trading Dashboard

A professional, responsive web application designed for Bitcoin traders that provides real-time market news, trading strategy guidance, and session timing alerts. 

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

## ⚠️ Disclaimer

**Trading involves substantial risk of loss and is not suitable for every investor.** This dashboard is for educational and informational purposes only. The creators are not responsible for any trading decisions made based on the information provided.

- Past performance is not indicative of future results
- Always do your own research
- Never invest more than you can afford to lose
- Consider consulting with a qualified financial advisor
