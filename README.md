# SNAP-Session-Zones-Reference-Levels

## Overview
The SNAP Session Zones + Reference Levels indicator is a TradingView Pine Script that maps the market by session, range, and reference levels. It helps identify where liquidity is likely resting above highs or below lows.

## Features

### Session Zones
- London session
- New York session
- Tokyo session
- Sydney session
- EU session
- US 9:30-10:30 session
- New Day Open session

### Reference Levels
- M0-M5 levels
- Daily Open
- Yesterday High/Low
- Last Week High/Low
- Average Daily Range (ADR)
- PSY Levels
- New Day Open Reference

### Climax Sessions
- Selling Climax Session detection
- Buying Climax Session detection
- RSI and volume-based identification

### **NEW: Macro Intervals** ✨
- Visual blue vertical line markers for four daily macro trading windows
- Automatic detection at 9:50 AM, 10:50 AM, 1:50 PM, and 2:50 PM ET
- Time labels for each interval
- Customizable line color, width, and extension
- Perfect for timing news events and identifying CISD (Change In State of Delivery)

See [MACRO_INTERVALS_GUIDE.md](MACRO_INTERVALS_GUIDE.md) for detailed information about the macro intervals feature.

## Getting Started

1. Add the indicator to your TradingView chart
2. Configure your preferred timezone (default: America/New_York)
3. Toggle session zones, reference levels, and macro intervals as needed
4. Customize colors and display settings to your preferences

## Documentation

- **[MACRO_INTERVALS_GUIDE.md](MACRO_INTERVALS_GUIDE.md)** - Comprehensive guide for using macro intervals for trading and analysis
