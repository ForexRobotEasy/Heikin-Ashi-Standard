# Heikin Ashi Standard Indicator ReadMe File

This code is an implementation of the Heikin Ashi Standard indicator for MetaTrader 4. The code is provided by Forex Robot Easy Team and can be found on their website [Forex Robot Easy](https://www.forexroboteasy.com).

## Indicator Settings

- `MA_Period` (default value: 14): The period used to calculate the moving average.

## Indicator Buffers

- `OpenBuffer[]`: Buffer to store the calculated open values.
- `CloseBuffer[]`: Buffer to store the calculated close values.
- `HighBuffer[]`: Buffer to store the calculated high values.
- `LowBuffer[]`: Buffer to store the calculated low values.

## Indicator Initialization

The `OnInit()` function is called once during the indicator initialization. In this function, the indicator settings and buffers are configured.

## Indicator Calculation

The `OnCalculate()` function is called for each new tick to calculate the indicator values. In this function, the Heikin Ashi Standard calculation is performed.

The Heikin Ashi calculation is as follows:

1. Calculate the average of the previous bar's open and close and store it in the `OpenBuffer`.
2. Calculate the average of the current bar's open, high, low, and close and store it in the `CloseBuffer`.
3. Calculate the maximum value among the current bar's high, `OpenBuffer`, and `CloseBuffer` and store it in the `HighBuffer`.
4. Calculate the minimum value among the current bar's low, `OpenBuffer`, and `CloseBuffer` and store it in the `LowBuffer`.

## Product Description

[Heikin Ashi Standard](https://forexroboteasy.com/forex-robot-review/heikin-ashi-standard-review-optimize-forex-with-custom-candles/) is a custom indicator designed to optimize forex trading using Heikin Ashi candles. 

Heikin Ashi candles are a type of Japanese candlestick charting technique that smooths out price fluctuations, making it easier to identify trends and reversals. This indicator calculates and displays the Heikin Ashi candles on the chart, providing traders with a visual representation of price action.

Some key features of Heikin Ashi Standard include:
- Easy to use: Simply add the indicator to your chart and it will automatically calculate and display the Heikin Ashi candles.
- Customizable: You can adjust the period used for calculating the moving average to suit your trading strategy.
- Clear signals: Heikin Ashi candles help to filter out noise and provide clearer signals for trend identification.

Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing the sample code that can work as described in the product. To find the official developer of this product, please refer to the MQL5 platform.
