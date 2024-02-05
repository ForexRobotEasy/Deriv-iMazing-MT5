# Deriv iMazing MT5

[![Build Status](https://img.shields.io/travis/username/repo.svg)](https://travis-ci.org/username/repo)

This is the code for the Deriv iMazing MT5 Expert Advisor. The code facilitates efficient trading in the forex market, optimizing progressively from 2020 to 2023. It implements high-frequency trade execution and enables trading of CFDs on synthetic indices in addition to standard forex trading. It also provides access to synthetic indices 24/7.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/deriv-imazing-mt5-review-optimized-forex-trading-software-2020-2023/). Please note that ForexRobotEasy is not the official developer of this product. We only show sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Installation and Usage

1. Copy the code into your MetaEditor.
2. Compile the code.
3. Attach the Expert Advisor to a chart in your MetaTrader 5 platform.
4. Adjust the necessary parameters, such as the symbols, trade volume, maximum trade count, desired profit percentage, and maximum drawdown percentage.
5. Start trading.

## Functionality

The Expert Advisor uses the Trade library to enable trading in the forex market. It sets up the necessary parameters, such as the expert magic number, market open settings, and trading symbol, during initialization.

During each tick, the Expert Advisor checks if enough bars are available for analysis. If there are enough bars, it calculates the desired number of profitable trades and the maximum allowed drawdown based on user-defined parameters.

Next, it performs trade analysis by iterating through a maximum trade count. For each trade, it calculates the entry and exit prices and checks if the trade is profitable. It also calculates the drawdown for each trade and keeps track of the current number of profitable trades and drawdown.

If the analysis is complete and the number of profitable trades meets the target and the drawdown is within the allowed limit, the Expert Advisor opens a trade with the desired volume.

The Expert Advisor also includes a deinitialization function that closes any open trades and prints a message upon deinitialization.

## Requirements

- MetaTrader 5 platform
- Trade library

## License

This code is licensed under the [MIT License](https://opensource.org/licenses/MIT).
