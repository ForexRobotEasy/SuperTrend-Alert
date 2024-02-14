# SuperTrend Alert

This code is an Expert Advisor (EA) that utilizes the SuperTrend indicator to detect trend shifts in the Forex market. The SuperTrend indicator is a popular technical analysis tool that helps traders identify potential entry and exit points based on the strength of a trend.

## SuperTrend Indicator Parameters

- ATRPeriod: The period used to calculate the Average True Range (ATR), which is the basis for the SuperTrend calculation.
- Multiplier: The multiplier applied to the ATR to determine the distance of the upper and lower bands from the price.

## Alert Parameters

- EnableAlerts: Set to true to enable pop-up alerts on trend shifts.
- EnableNotifications: Set to true to enable push notifications on trend shifts.
- EnableEmails: Set to true to enable email notifications on trend shifts.

## Color Scheme Parameters

- UpTrendColor: The color used to display an upward trend.
- DownTrendColor: The color used to display a downward trend.
- NeutralColor: The color used to display a neutral or non-trending market.

The EA initializes the SuperTrend indicator with the specified parameters in the `OnInit()` function. It also sets the color scheme for the chart using the `ChartSetInteger()` function.

In the `OnDeinit()` function, the EA resets the chart color scheme to the default settings.

The `OnTick()` function is called on each tick of the market. It retrieves the upper and lower bands of the SuperTrend indicator using the `IndicatorGetDouble()` function. Then, it checks for trend shift indications by comparing the current price with the upper and lower bands. If a trend shift is detected, the EA generates alerts, notifications, and emails based on the enabled parameters.

Please note that this code is a sample provided by Forex Robot Easy Team and is not the official product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, visit [Forex Robot Easy - SuperTrend Alert Review](https://forexroboteasy.com/forex-robot-review/supertrend-alert-review-enhance-your-trading-with-this-indicator/).
