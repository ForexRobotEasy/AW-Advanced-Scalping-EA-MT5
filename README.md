# AW Advanced Scalping EA MT5

This is a sample code for the AW Advanced Scalping EA MT5 developed by the Forex Robot Easy Team. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in the product.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/aw-advanced-scalping-ea-mt5-review-automated-forex-trading-tool/).

## Description

The AW Advanced Scalping EA MT5 is an automated forex trading tool designed for scalping strategies. It utilizes a self-developed oscillator to identify potential trading opportunities and execute trades accordingly.

### Input Parameters

- **LotSize**: Initial lot size for trading.
- **OscillatorPeriod**: Period for the self-developed oscillator.
- **RecoveryFactor**: Recovery factor for the overlap recovery algorithm.
- **StepSize**: Step size for adjusting orders.
- **AllowManualOrders**: Option to allow manual orders.

### Global Variables

- **trade**: Trade object for executing orders.
- **oscillatorBuffer[]**: Buffer for storing oscillator values.
- **lastOrderType**: Variable to store the type of the last order.

## Custom Initialization Function

The `OnInit()` function initializes the oscillator buffer and calculates oscillator values for each bar.

## Custom Start Function

The `OnStart()` function is responsible for initiating trades based on the calculated oscillator values.

- It calculates the lot size using the `CalculateLotSize()` function.
- It checks for potential losses and initiates overlap recovery if necessary.
- It checks for price reversals and initiates trading accordingly.

## Custom Function to Calculate Lot Size

The `CalculateLotSize()` function calculates the lot size based on the current market trend against the trader. If the last order type is a buy and the oscillator value is negative, or if the last order type is a sell and the oscillator value is positive, the lot size is adjusted using the recovery factor.

For more information about this product and to find the official developer, please refer to the [MQL5](https://www.mql5.com/) website.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/aw-advanced-scalping-ea-mt5-review-automated-forex-trading-tool/).
