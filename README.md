# 📊 Smart Position Sizer for TradingView

[![TradingView](https://img.shields.io/badge/TradingView-Script-blue.svg)](https://www.tradingview.com/)
[![PineScript](https://img.shields.io/badge/PineScript-v6-green.svg)](https://www.tradingview.com/pine-script-docs/en/v6/Introduction.html)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Forex](https://img.shields.io/badge/Market-Forex-orange.svg)](https://www.tradingview.com/symbols/EURUSD/)

> A professional risk management tool for Forex traders that calculates optimal position sizes based on account balance, risk parameters, and price levels.

![Position Sizer Demo](https://raw.githubusercontent.com/uncogeek/position-sizer/master/screenshot.png)

## ✨ Features

- **Interactive Price Levels**: Easily adjust entry, stop loss, and take profit levels directly on the chart
- **Auto-Initialization**: Automatically sets up at current price when first loaded
- **Visual Clarity**: Clear labels show exact prices at the end of each line
- **Risk Management**: Calculate position size based on account risk percentage
- **Reward Analysis**: Shows potential reward in both pips and USD
- **Margin Calculation**: Displays used and free margin based on leverage
- **Automatic Direction Detection**: Identifies long/short positions based on stop loss placement
- **Risk:Reward Visualization**: Clearly displays R:R ratio for trade evaluation

## 🚀 Installation

1. Open TradingView and create a new Pine Script indicator
2. Delete the default code
3. Copy and paste the entire code from `position_sizer.pine`
4. Click "Save" and name your indicator
5. Click "Add to Chart" to use the position sizer

## 📖 How It Works

The Position Sizer helps traders maintain proper risk management by:

1. Calculating the appropriate lot size based on your risk tolerance
2. Visualizing entry, stop loss, and take profit levels directly on the chart
3. Providing a comprehensive table with all risk metrics
4. Updating calculations in real-time as you adjust price levels

### Risk Management Panel

| Metric | Description |
|--------|-------------|
| Direction | Automatically detects long/short based on SL placement |
| Entry Price | Your entry point for the trade |
| Stop Loss | Where your trade will exit if the market moves against you |
| Take Profit | Your profit target |
| Risk (USD) | Exact dollar amount at risk |
| Reward (USD) | Potential profit in dollars |
| Risk (pips) | Distance from entry to stop loss in pips |
| Reward (pips) | Distance from entry to take profit in pips |
| Lot Size | Calculated position size to match your risk percentage |
| R:R Ratio | Reward to Risk ratio |
| Margin Used | Amount of account margin allocated to this position |
| Free Margin | Remaining available margin in your account |

## 🔧 Customization

You can easily customize the Position Sizer through the inputs panel:

- **Account Settings**:
  - Account Balance: Your trading account size
  - Risk Percentage: Your risk tolerance per trade (default 1%)
  - Leverage: Your broker's leverage (default 50:1)

- **Price Levels**:
  - Entry/SL/TP: Adjust directly on chart or through inputs panel
  - Colors: Customize the color of each line

## 💡 Usage Tips

- **Optimal Risk Management**: Keep risk percentage between 1-2% per trade
- **Position Direction**: For long positions, place SL below entry; for shorts, place SL above entry
- **Visual Analysis**: Use the clear labels to precisely measure distance in price
- **Realistic Goals**: Aim for R:R ratios of at least 1.5:1 for sustained profitability

## 📈 Example Scenarios

### Conservative EUR/USD Day Trading
- Account: $10,000
- Risk: 1% ($100)
- Stop Loss: 20 pips
- Position Size: 0.50 lots

### Aggressive EUR/USD Trend Trading
- Account: $10,000
- Risk: 2% ($200)
- Stop Loss: 40 pips
- Position Size: 0.50 lots

## 🔒 Requirements

- TradingView Pro account or higher
- Basic understanding of trading concepts and risk management

## 🤝 Contributing

Feel free to fork this project and submit pull requests with enhancements. Some ideas for improvements:

- Add support for additional currency pairs with different pip values
- Implement trailing stop calculation
- Add break-even calculator
- Create multi-position portfolio risk manager

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<p align="center">
  <b>Developed with ❤️ for responsible traders</b><br>
  <i>Note: Trading involves risk. Always use proper risk management.</i>
</p>
