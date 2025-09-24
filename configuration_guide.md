# MurshidFx Premium V1.0 - Configuration Guide

## Quick Start Settings

### Minimalist Setup (Clean Chart)
```
Main Controls:
- Show HTF Candles: ✓
- Show Interval Separators: ✗
- Show Open Price Lines: ✓

Display Settings:
- Historical Display Count: 3

HTF Candles:
- Show Timeframe Labels: ✓

Market Structure:
- Show Fair Value Gaps: ✗
- Show Volume Imbalance: ✗
- Show Sweeps: ✗
- Show Midpoints: ✓

Dashboard:
- Show Professional Dashboard: ✓
- Position: top-right
```

### Full Analysis Setup
```
Main Controls:
- Show HTF Candles: ✓
- Show Interval Separators: ✓
- Show Open Price Lines: ✓

Display Settings:
- Historical Display Count: 5

Market Structure:
- Show Fair Value Gaps: ✓
- Show Volume Imbalance: ✓
- Show Sweeps: ✓
- Show Midpoints: ✓

All visual features enabled for comprehensive analysis
```

### Day Trading Setup
```
Recommended Timeframes: 1m, 3m, 5m charts

Settings:
- Historical Display Count: 3-4
- Candle Padding: 15-20
- Show Sweeps: ✓ (important for intraday)
- Show Midpoints: ✓
- Show Open Price Lines: ✓
- Show Mid-Line: ✓ (for range trading)
```

### Swing Trading Setup
```
Recommended Timeframes: 15m, 30m, 1H charts

Settings:
- Historical Display Count: 5-7
- Candle Padding: 25-30
- Show Fair Value Gaps: ✓
- Show Volume Imbalance: ✓
- Show Interval Separators: ✓
```

## Color Schemes

### Dark Theme
```
Bullish Candle: #81c784 (light green)
Bearish Candle: #000000 (black)
Frame Color: #000000 (black)
Separator Lines: #808080 (gray)
Open Price Line: #000000 (black)
Mid-Line: #ff0000 (red, 20% opacity)
FVG Color: #808080 (gray, 80% opacity)
Dashboard Background: #ffffff (white, 5% opacity)
```

### Light Theme
```
Bullish Candle: #26a69a (teal)
Bearish Candle: #ef5350 (red)
Frame Color: #424242 (dark gray)
Separator Lines: #9e9e9e (light gray)
Open Price Line: #1976d2 (blue)
Mid-Line: #ff6f00 (orange)
Dashboard Background: #000000 (black, 10% opacity)
```

## Spacing Recommendations

### For 1920x1080 Resolution
```
Candle Padding: 22
Space Between Candles: 1
Space Between HTF Sets: 10
Candle Width: 1
```

### For 4K Resolution
```
Candle Padding: 30-35
Space Between Candles: 2
Space Between HTF Sets: 15
Candle Width: 2
```

### For Mobile/Tablet
```
Candle Padding: 15
Space Between Candles: 1
Space Between HTF Sets: 8
Candle Width: 1
```

## Feature Combinations

### Price Action Focus
- HTF Candles: ON
- Sweeps: ON
- Midpoints: ON
- Everything else: OFF

### Structure Trading
- HTF Candles: ON
- Interval Separators: ON
- Open Price Lines: ON
- Mid-Line: ON
- FVG: ON

### Scalping Setup
- HTF Candles: ON (display count: 2-3)
- Open Price Lines: ON
- Sweeps: ON
- Dashboard: ON (for timing)

## Performance Tips

1. **Reduce Display Count**: Lower numbers (3-5) improve performance
2. **Disable Unused Features**: Turn off FVG/Volume Imbalance if not needed
3. **Simplify Visuals**: Use solid lines instead of dotted for better rendering
4. **Limit HTF Sets**: The indicator performs best with 1-3 active HTF sets

## Common Issues & Solutions

### Issue: Cluttered Chart
**Solution**: Reduce display count, increase spacing, disable some features

### Issue: Slow Performance
**Solution**: Lower display count, disable market structure features, use fewer HTF sets

### Issue: Overlapping Elements
**Solution**: Increase padding values, adjust candle width, reposition dashboard

### Issue: Can't See Labels
**Solution**: Check label colors against background, increase label size, verify "Show Timeframe Labels" is enabled