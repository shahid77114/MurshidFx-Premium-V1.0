# MurshidFx Premium V1.0 - Bug Report & Issues

## Critical Bugs

### 1. **Array Access Without Bounds Checking**
**Location**: Multiple locations in Helper methods
**Issue**: Accessing array elements without checking if index is valid
```pinescript
// BUG: No validation that monthVal is within bounds
monthStr = array.get(months, monthVal - 1)
```
**Impact**: Can cause runtime errors if monthVal is invalid

### 2. **Division by Zero Potential**
**Location**: `ValidTimeframe` method
```pinescript
// BUG: No check for n1 or n2 being zero
if n1 < n2 and math.round(n2 / n1) == n2 / n1
```
**Impact**: Script crash if timeframe.in_seconds returns 0

### 3. **Uninitialized Array Access**
**Location**: `CheckSweeps` and `CheckMidpoints` methods
```pinescript
// BUG: Accessing sweeps array without null check
if curr_candle.sweeps.size() > 0
```
**Impact**: Null reference errors

### 4. **Memory Leaks**
**Location**: Throughout the code
**Issue**: Creating visual objects without proper cleanup in some paths
**Impact**: Performance degradation over time

### 5. **Timezone Inconsistency**
**Location**: Dashboard vs HTF calculations
**Issue**: Dashboard uses chart timezone while HTF uses NY timezone
**Impact**: Time display mismatches

## Performance Issues

### 1. **Redundant Array Size Calculations**
**Location**: Multiple methods
```pinescript
// Called multiple times in same scope
for i = 0 to array.size(candles) - 1
```

### 2. **Inefficient Object Creation**
**Location**: `Monitor` method
**Issue**: Creating new objects on every update without pooling

### 3. **Unnecessary Processing**
**Location**: `DrawOpenPriceLines` method
**Issue**: Clears and recreates lines even when disabled

## Logic Issues

### 1. **HTF Setting Overwrite**
**Location**: Section 6 execution
**Issue**: HTF settings are overwritten on each bar update
```pinescript
// This runs on every bar, overwriting user settings
htf1.settings.htf := higherTF
```

### 2. **Incomplete Sweep Validation**
**Location**: `CheckSweeps` method
**Issue**: Doesn't validate if previous candle exists before accessing

### 3. **Midpoint Calculation Timing**
**Location**: `CheckMidpoints` method
**Issue**: Deletes and recreates midpoints unnecessarily

### 4. **Label Position Conflicts**
**Location**: Open price and mid-line labels
**Issue**: Labels can overlap when both are enabled

## Edge Cases Not Handled

### 1. **Weekend/Holiday Gaps**
**Issue**: No handling for market closures
**Impact**: Incorrect time calculations

### 2. **Symbol Changes**
**Issue**: No validation when switching symbols
**Impact**: Stale data display

### 3. **Timeframe Restrictions**
**Issue**: No validation for incompatible timeframe combinations
**Impact**: Incorrect displays on some timeframes

### 4. **Max Object Limits**
**Issue**: No tracking of Pine Script object limits
**Impact**: Script can fail when limits exceeded

## Data Integrity Issues

### 1. **Candle Data Updates**
**Location**: `Update` method
**Issue**: Updates current candle without validating data changes

### 2. **Historical Data Loading**
**Issue**: No validation for incomplete historical data

### 3. **Time Series Consistency**
**Issue**: No checks for time series gaps or duplicates

## User Experience Issues

### 1. **Setting Validation**
**Issue**: No validation for conflicting settings
**Example**: Negative spacing values accepted

### 2. **Error Messages**
**Issue**: No user-friendly error messages
**Impact**: Difficult to troubleshoot issues

### 3. **Performance Warnings**
**Issue**: No warnings when settings may impact performance

## Security/Safety Issues

### 1. **Input Validation**
**Issue**: User inputs not sanitized
**Example**: Custom text inputs could break display

### 2. **Resource Limits**
**Issue**: No protection against resource exhaustion

## Recommended Priority

1. **Critical**: Array bounds checking, null checks
2. **High**: Division by zero, memory leaks
3. **Medium**: Performance optimizations, logic fixes
4. **Low**: UX improvements, edge cases