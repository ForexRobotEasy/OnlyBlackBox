# OnlyBlackBox Trading Robot

**Developer:** Forex Robot Easy Team

**Website:** [forexroboteasy.com](https://forexroboteasy.com/)

This code is a sample implementation of the OnlyBlackBox Trading Robot. It is a simple trading robot that executes buy and sell trades based on a specific trading logic. 

## Functionality

The trading robot uses the MetaTrader 5 platform and requires the following libraries:

- Trade.mqh
- TimeSeries.mqh
- ArrayInt.mqh
- ArrayDouble.mqh
- Conversion.mqh
- DateTime.mqh
- Math.mqh

The robot is designed to trade the 'US30' symbol on the H1 timeframe. It uses a fixed risk percentage and two take profit levels. The risk percentage is set to 1% of the account balance, and the take profit levels are calculated based on partial percentages (0.5% and 1% of the current price).

The trading logic is executed in the `OnStart()` and `OnTrade()` functions. The `OnStart()` function is called when the robot starts, and it refreshes the time series data and executes the trading logic. The `OnTrade()` function is called whenever a trade event occurs, and it also executes the trading logic.

The trading logic is as follows:

1. Calculate the lot size based on the risk percentage and account balance.
2. Calculate the stop loss and take profit levels based on the current price and the partial percentages.
3. If the current price is higher than the previous open price, open a buy trade with the calculated lot size, stop loss, and take profit levels.
4. If the current price is lower than the previous open price, open a sell trade with the calculated lot size, stop loss, and take profit levels.

The `CloseAllTrades()` function is used to close all open trades.

## Usage

To use this trading robot, follow these steps:

1. Install MetaTrader 5 platform.
2. Open the MetaEditor and create a new Expert Advisor.
3. Copy and paste the provided code into the Expert Advisor file.
4. Include the necessary libraries and define the constants.
5. Initialize the trading class and objects.
6. Implement the necessary functions to calculate lot size and take profit levels.
7. Implement the functions to open buy and sell trades, close all trades, and execute the trading logic.
8. Initialize the trading robot in the `OnInit()` function.
9. Start the trading robot in the `OnStart()` function.
10. Handle trading events in the `OnTrade()` function.
11. Compile and run the Expert Advisor on the MetaTrader 5 platform.

**Note:** ForexRobotEasy is not the official developer of this product. This code is provided as a sample implementation that can work as described in the product. To find the official developer of this product, please refer to the [MQL5](https://www.mql5.com/) website.

## Product Description

The OnlyBlackBox Trading Robot is a powerful tool developed by the Forex Robot Easy Team. It is designed to automate the trading process and provide smart money forex trading strategies. With its advanced algorithm, the robot analyzes market conditions and executes trades based on predefined rules.

Key Features:

- Works on the MetaTrader 5 platform.
- Supports trading on the 'US30' symbol with the H1 timeframe.
- Implements a fixed risk percentage for optimal money management.
- Calculates take profit levels based on partial percentages.
- Executes buy and sell trades based on a simple trading logic.
- Provides the ability to close all open trades.
- Easy to use and customize.

With the OnlyBlackBox Trading Robot, traders can take advantage of the smart money forex trading strategies and optimize their trading performance. Explore the full potential of this product and enhance your trading experience.

For detailed reviews and trading results of this product, please visit the [product review page](https://forexroboteasy.com/forex-robot-review/onlyblackbox-review-smart-money-forex-trading-with-mt5/).

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code implementation that can work as described in the product. To find the official developer of this product, please use the [MQL5](https://www.mql5.com/) website.
