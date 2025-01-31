---
created: '2025-01-31T06:27:03.942971'
modified: '2025-01-31T06:27:03.942977'
source: '[[Support-and-Resistance]]'
hierarchy:
- Trading
- Files
tags: []
summary: ''
concepts: []
ai_generated: true

---

# ATR(Average True Range):

## Context Path
Trading > Files

## Content
> **AI Generated Content**
 # Average True Range (ATR) in Trading

## Core Definitions

### What is ATR?
Average True Range (ATR) is a technical analysis indicator that measures market volatility by decomposing the entire range of an asset price for that period. It was developed by J. Welles Wilder Jr. and introduced in his 1978 book, "New Concepts in Technical Trading Systems."

### Formula and Calculation
The True Range (TR) is calculated as follows:
\[ \text{True Range} = \max[\text{High} - \text{Low}, |\text{High} - \text{Close}|, |\text{Low} - \text{Close}|] \]

The ATR is then the simple moving average of the TR over a specified period (usually 14 days).
\[ \text{ATR} = \frac{\sum_{i=1}^{n} \text{TR}_i}{n} \]
where \( n \) is the number of periods.

### Key Features
- **Volatility Measure**: ATR helps traders understand how much an asset's price is fluctuating.
- **Risk Management**: Traders use ATR to set stop-loss orders and determine position sizes.
- **Trend Indicator**: High ATR values can indicate a strong trend, while low values might suggest a range-bound market.

## Practical Applications

### Risk Management
ATR is widely used for setting stop-loss orders. For example, if the current ATR is 0.5, a trader might place a stop-loss order 0.5 points below the entry price to manage risk effectively.

### Position Sizing
Traders use ATR to determine the number of shares or contracts to trade based on their risk tolerance. For instance, if a trader is willing to risk $1000 and the current ATR is $0.25, they might buy 4000 shares (since \( \$1000 / \$0.25 = 4000 \)).

### Identifying Market Conditions
- **High ATR**: Indicates high volatility and a strong trend. Traders may look for breakouts or pullbacks in this scenario.
- **Low ATR**: Suggests low volatility and range-bound conditions. Traders might consider range trading strategies.

### Entry and Exit Points
ATR can help traders identify optimal entry and exit points. For example, if the price moves 1.5 times the ATR from a recent high or low, it could signal a potential reversal point.

## Relationships to Parent Concepts

### Volatility
ATR is fundamentally linked to the concept of volatility in finance. It measures how much and how quickly prices change over time, providing insights into market conditions.

### Technical Analysis
As a technical analysis tool, ATR complements other indicators such as Relative Strength Index (RSI), Moving Averages (MA), and Bollinger Bands. Traders often use ATR in conjunction with these tools for more comprehensive analyses.

### Risk Management Strategies
ATR is integral to various risk management strategies, including the use of stop-loss orders and position sizing techniques. It helps traders quantify risk and make informed decisions.

## Simple Examples

### Example 1: Calculating ATR
Assume the following closing prices for a stock over five days:
- Day 1: High = $50, Low = $48, Close = $49
- Day 2: High = $51, Low = $47, Close = $48.5
- Day 3: High = $52, Low = $46, Close = $49
- Day 4: High = $53, Low = $45, Close = $48
- Day 5: High = $54, Low = $44, Close = $47

Calculating the True Range for each day:
- Day 1: TR = max[2, 1, 1] = 2
- Day 2: TR = max[3.5, 2.5, 2.5] = 3.5
- Day 3: TR = max[6, 3, 3] = 6
- Day 4: TR = max[8, 7, 7] = 8
- Day 5: TR = max[10, 9, 9] = 10

The 5-day ATR is:
\[ \text{ATR} = \frac{2 + 3.5 + 6 + 8 + 10}{5} = \frac{29.5}{5} = 5.9 \]

### Example 2: Setting Stop-Loss Orders
If the current ATR is $1, a trader with a risk tolerance of $500 might set a stop-loss order $500/$1 = 500 points below the entry price to manage their risk effectively.

### Example 3: Identifying Market Conditions
In a scenario where the ATR is consistently high (e.g., above 2 for several days), traders might anticipate a strong trend and look for potential breakouts or pullbacks. Conversely, if the ATR remains low (e.g., below 0.5), they might consider range trading strategies.

By understanding and applying ATR in these ways, traders can better manage risk, identify market conditions, and make more informed trading decisions.

## Related Concepts
