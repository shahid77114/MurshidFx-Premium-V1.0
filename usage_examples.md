# MurshidFx Premium V1.0 - Usage Examples

## Example 1: Intraday Trading on 5-Minute Chart

### Scenario
You're day trading ES (S&P 500 futures) on a 5-minute chart and want to see 1-hour candles for context.

### Configuration
1. **Main Controls**
   - Show HTF Candles: ✓
   - Show Interval Separators: ✓
   - Show Open Price Lines: ✓

2. **Display Settings**
   - Historical Display Count: 4 (shows last 4 hourly candles)

3. **Key Features to Enable**
   - Show Sweeps: ✓ (identify stop hunts)
   - Show Midpoints: ✓ (potential reversal levels)
   - Show Mid-Line: ✓ (range midpoint for mean reversion)

### How to Use
- **Entry Signal**: Look for sweeps of previous hourly highs/lows that fail to continue
- **Target**: Previous hourly candle midpoints or open prices
- **Stop Loss**: Beyond the sweep level
- **Context**: Use interval separators to identify the hourly range

## Example 2: Swing Trading on Daily Chart

### Scenario
Trading stocks on daily charts, wanting to see weekly and monthly context.

### Configuration
1. **Timeframe**: Daily chart → Shows Weekly candles automatically
2. **Historical Display Count**: 6-8 (shows 6-8 weeks of history)
3. **Enable**:
   - Fair Value Gaps: ✓
   - Volume Imbalance: ✓
   - Show Open Price Lines: ✓

### Trading Approach
- **Weekly FVGs**: Look for price to return to weekly fair value gaps
- **Open Price Magnets**: Weekly opens often act as magnets
- **Structure**: Use weekly candle patterns for bias

## Example 3: Scalping on 1-Minute Chart

### Scenario
Fast scalping on 1-minute charts with 15-minute structure.

### Configuration
```
Historical Display Count: 3
Candle Padding: 15 (keeps chart clean)
Show Sweeps: ✓
Show Open Price Lines: ✓
Dashboard Position: top-right
```

### Quick Rules
1. **Bullish Bias**: Current price above 15m open + previous 15m was bullish
2. **Bearish Bias**: Current price below 15m open + previous 15m was bearish
3. **Entry**: On sweep of 15m high/low that fails
4. **Exit**: Quick 10-20 tick moves

## Example 4: Range Trading

### Scenario
Trading ranging markets using interval boundaries.

### Setup
- Enable all separator features
- Show Mid-Line: ✓
- Historical Display Count: 5

### Strategy
1. **Identify Range**: Use interval separators to see clear ranges
2. **Entry Points**:
   - Long at interval low + open price confluence
   - Short at interval high + resistance
3. **Targets**: Mid-line or opposite boundary
4. **Stop**: Outside range boundaries

## Example 5: News Trading

### Scenario
Trading around scheduled news events.

### Configuration Focus
- Dashboard: ✓ (watch countdown timer)
- Open Price Lines: ✓ (pre-news reference)
- Historical Display: 2-3 (keep it simple)

### Approach
1. **Mark Pre-News Levels**: Note HTF open and mid prices
2. **Wait for News**: Watch how price reacts to these levels
3. **Trade the Reaction**: 
   - Break and hold above = bullish
   - Rejection at levels = fade the move

## Example 6: Multiple Timeframe Confluence

### Chart Setup
- 15-minute chart
- Shows: 1H, 4H, and Daily candles

### Looking for Confluence
1. **Bullish Setup**:
   - Price above Daily open ✓
   - Price above 4H open ✓
   - Price above 1H open ✓
   - Recent 1H candle bullish ✓

2. **Entry**: Pullback to 1H open or midpoint
3. **Target**: Previous day high or 4H candle high
4. **Stop**: Below confluence of opens

## Tips for All Setups

### Visual Clarity
- Adjust spacing based on your monitor size
- Use contrasting colors for different timeframes
- Keep enabled features to what you actively use

### Performance
- Lower display count for faster updates
- Disable market structure features if not needed
- Use solid lines for better performance

### Best Practices
1. **Start Simple**: Enable one HTF set first
2. **Add Gradually**: Add features as you understand them
3. **Document**: Keep notes on which setups work best
4. **Backtest**: Use bar replay to practice setups
5. **Adapt**: Adjust settings based on market conditions

## Common Patterns to Watch

### 1. **Open Test and Reject**
- Price tests previous HTF open
- Strong rejection candle forms
- Enter in direction of rejection

### 2. **Midpoint Bounce**
- Price reaches previous HTF midpoint
- Shows deceleration
- Enter for continuation or reversal

### 3. **Sweep and Reverse**
- Quick sweep of HTF high/low
- Immediate reversal back inside
- Enter in reversal direction

### 4. **FVG Fill**
- Price enters HTF fair value gap
- Shows reaction at gap boundaries
- Trade the reaction direction

### 5. **Multi-Timeframe Alignment**
- All HTF candles same color (trend)
- Price pulls back to nearest open
- Enter in trend direction