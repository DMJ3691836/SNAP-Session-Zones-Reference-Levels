# Macro Intervals Feature Guide

## Overview

The **Macro Intervals** feature has been added to the SNAP Session Zones + Reference Levels indicator to visually mark critical trading times when significant market moves often occur. These 20-minute intervals are marked with blue vertical lines and labeled on your trading chart.

## What Are Macro Intervals?

Macro intervals are 20-minute trading windows that occur four times daily, during which high-impact news announcements and significant market moves typically occur. These intervals often mark changes in delivery state (CISD - Change In State of Delivery).

### The Four Daily Macro Intervals:

1. **9:50-10:10 AM ET** - Morning macro interval
2. **10:50-11:10 AM ET** - Mid-morning macro interval
3. **1:50-2:10 PM ET** - Afternoon macro interval
4. **2:50-3:10 PM ET** - Late afternoon macro interval

## Market Impact

When high-impact news drivers and seasonal trends align with directional bias during macro intervals, you can expect stronger price movements within these windows. Key announcements often timed to these windows include:
- FOMC announcements
- CPI releases
- BOJ (Bank of Japan) reports
- BOE (Bank of England) statements
- Federal Reserve statements

## How to Use

### Enabling the Feature

1. Open the SNAP Session Zones indicator settings on your TradingView chart
2. Scroll down to the **"Macro Intervals"** input group
3. Toggle **"Show macro intervals"** to ON (default: enabled)

### Customizing the Display

In the **Macro Intervals** settings group, you can customize:

| Setting | Description | Default |
|---------|-------------|---------|
| **Show macro intervals** | Enable/disable macro interval lines | ON |
| **Macro interval colour (Blue)** | Line color picker | Blue (RGB 0, 100, 255) |
| **Macro interval line width** | Thickness of vertical lines (1-5) | 2 |
| **Macro interval extension candles right** | How many bars to extend lines to the right (0-200) | 20 |

### Visual Appearance

- **Blue vertical lines** are drawn at the exact start time of each macro interval (9:50 AM, 10:50 AM, 1:50 PM, 2:50 PM ET)
- **Time labels** are positioned above each line showing the interval range (e.g., "9:50-10:10")
- Lines extend through the entire visible chart height using the `extend.both` setting
- Each line remains visible for the configured extension period

## Trading Strategy Applications

### 1. News Event Timing
- Align your trading calendar to these macro intervals
- Prepare entry/exit strategies before these times
- Watch for volatility spikes during these windows

### 2. Market Structure Analysis
- Use macro intervals to identify structural support/resistance breaks
- Monitor CISD (Change In State of Delivery) at these times
- Track institutional order flow during these periods

### 3. Session Breakout Trading
- Combine macro intervals with session zones
- Look for breakouts from New Day Open or London session ranges at macro times
- Use macro intervals to validate trend changes

### 4. Risk Management
- Tighten stops before macro intervals
- Reduce position size during these periods
- Avoid opening new positions if major news is expected

## Technical Implementation

The macro intervals feature:
- Detects the current bar's hour and minute in real-time
- Creates vertical lines when the exact minute matches (9:50, 10:50, 13:50, 14:50)
- Prevents duplicate lines by tracking the last macro interval bar processed
- Automatically manages old lines (keeps maximum 100 entries)
- Works seamlessly with all other SNAP indicator features

## Notes

- **Timezone**: Macro intervals are calculated in **America/New_York (ET)** timezone
- **Compatibility**: Works with all chart timeframes (recommended: 1m, 5m, 15m)
- **Performance**: Efficiently manages indicator resources by limiting stored lines
- **Display**: Lines are extended both upward and downward for optimal visibility

## Example Workflow

1. Enable the SNAP Session Zones indicator
2. Turn ON "Show macro intervals"
3. Set your chart timezone to ET (America/New_York)
4. Watch for blue lines appearing at the designated times
5. Use these markers to time your trades or news event preparation
6. Combine with other SNAP features (session zones, reference levels) for comprehensive analysis

---

*For more information about the SNAP Session Zones indicator, refer to the main README.md file.*
