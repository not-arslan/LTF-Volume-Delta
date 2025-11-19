# LTF-Volume-Delta

LTF-Volume-Delta is a TradingView indicator that reconstructs intrabar buying and selling pressure using lower-timeframe data. It calculates Up Volume, Down Volume, and Volume Delta through `ta.requestUpAndDownVolume()`, giving a clearer view of directional volume inside each candle.

The indicator automatically selects an optimal lower timeframe, with the option to manually override for users who want more precision or better historical depth.

## Features

- Calculates Up Volume, Down Volume, and Delta using lower-timeframe reconstruction
- Automatic adaptive lower timeframe selection
- Optional manual LTF input
- Column-style visualization for up and down volume
- Delta marker for identifying buying vs selling dominance
- Volume availability check with clear error prompts

## How It Works

The script analyzes lower-timeframe candles to estimate how much volume occurred during upward vs. downward movement.  
It outputs:
- **Up Volume:** volume during upward price moves  
- **Down Volume:** volume during downward moves  
- **Delta:** net difference between the two  

This provides a more detailed view of intrabar order flow and trend strength.

## File Structure

- `ltf-volume-delta.pine` — TradingView Pine Script
- `LICENSE` — MIT License
- `README.md` — Documentation

## License

Released under the **MIT License**.  
Copyright (c) 2025 **not-arslan**

Refer to the `LICENSE` file for full text.
