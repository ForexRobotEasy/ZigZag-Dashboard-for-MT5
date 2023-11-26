# ZigZag Dashboard for MT5

This code is a sample implementation of the ZigZag Dashboard indicator for MetaTrader 5 (MT5). The ZigZag Dashboard is a powerful tool that helps traders identify market trends and reversals. It allows users to monitor multiple currency pairs and timeframes simultaneously.

## Developer Information

- Developer's site: [forexroboteasy.com](https://forexroboteasy.com)
- Development by: Forex Robot Easy Team

## Table of Contents

- [Include Files](#include-files)
- [Global Variables](#global-variables)
- [Indicator Initialization Function](#indicator-initialization-function)
- [Indicator Deinitialization Function](#indicator-deinitialization-function)
- [Indicator Calculation Function](#indicator-calculation-function)

## Include Files

The code includes the `Trade.mqh` file, which provides functions for performing trading operations.

## Global Variables

- `g_symbol`: Stores the symbol for which the indicator is applied.
- `g_tf`: Stores the timeframe for which the indicator is applied.

## Indicator Initialization Function

The `OnInit()` function is called when the indicator is initialized. In this function, the symbol and timeframe are set. The indicator is then added to the chart using the `ChartIndicatorAdd()` function.

## Indicator Deinitialization Function

The `OnDeinit()` function is called when the indicator is removed from the chart. In this function, the indicator is removed from the chart using the `ChartIndicatorDelete()` function.

## Indicator Calculation Function

The `OnCalculate()` function is called for every new tick and is responsible for calculating the indicator values. In this function, the ZigZag data is obtained using the `IndicatorGetValues()` function. The last movement height, number of bars in the movement, and the breaking of the previous ZigZag point are calculated based on the ZigZag data and the price data.

The market direction is determined by comparing the current closing price with the ZigZag data. The calculated information is then displayed on the chart using the `Comment()` function.

## Product Description

This code represents a sample implementation of the ZigZag Dashboard indicator for MT5. The ZigZag Dashboard is a versatile and powerful tool that allows traders to monitor multiple currency pairs and timeframes simultaneously. It helps identify market trends and reversals, providing valuable insights for trading decisions.

Please note that ForexRobotEasy is not the official developer of this product. We only provide this sample code to demonstrate how the indicator can work. To find the official developer of this product, please refer to the [MQL5](https://www.mql5.com) website.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-zigzag-dashboard-for-mt5-multicurrency-and-multitimeframe-forex-software/).
