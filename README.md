# EasyTrade 1.0
Risk Management System

MQL5 Trade Loss Calculator

Overview

This MQL5 script calculates the potential loss per trade based on user input for lot size, entry price, and stop-loss price. It helps traders estimate risk before entering a trade by considering:

Lot size: The volume of the trade (user input).

Entry price: The price at which the trade is opened (user input).

Stop loss (SL): The price level at which the trade will be closed (user input).

Tick value: The monetary value of a pip in the account currency.

Risk calculation formula:

Loss = Lot Size * Tick Value * abs(Entry Price - Stop Loss Price) / Tick Size

Features

Allows manual input of lot size, entry price, and stop loss price.

Fetches trading symbol properties (tick value and tick size).

Computes the monetary risk per trade in USD.

Outputs the estimated loss in the terminal.

Installation

Open MetaTrader 5.

Go to File > Open Data Folder.

Navigate to MQL5\Scripts.

Copy and paste the TradeLossCalculator.mq5 script into this folder.

Restart MetaTrader 5 or refresh the Navigator panel.

Usage

Open the MetaTrader 5 terminal.

Attach the script to a chart.

Enter the lot size, entry price, and stop loss price when prompted.

Run the script to see the potential loss calculation in USD displayed in the terminal.

Example

If you input 1 lot with an entry price of 1.1000 and a stop loss price of 1.0950 on EUR/USD:

Enter lot size: 1.0
Enter entry price: 1.1000
Enter stop loss price: 1.0950
Potential loss for Lot Size 1.00, Entry Price 1.1000, and SL at 1.0950: 500.00 USD

This means you risk $500 if the trade hits stop loss.

Future Enhancements

Add risk percentage-based lot sizing.

Include risk-reward ratio calculations.

Create a GUI version for easy input.

License

This project is open-source. Feel free to modify and use it for personal or educational purposes.
