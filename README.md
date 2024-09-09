# Algorithmic Trading Strategy: RSI-Based Model with Price Pattern Recognition

## Languages & Libraries:
- **Python**: The primary language used for data manipulation, feature engineering, and the creation of trading simulations.
- **Pandas**: Utilized for data preprocessing, cleaning, and feature creation. Key operations include calculating percentage price changes (PC%) and generating financial indicators like the Relative Strength Index (RSI).
- **Numpy**: Used to manage numerical operations, particularly for RSI computation and handling array-based calculations.
- **Matplotlib & Seaborn**: Employed for visualizing data trends, allowing for insight into financial patterns and results.
- **Collections & Itertools**: Leveraged to create and manipulate iterators for efficient dataset traversal, as well as manage the holding periods and pattern recognition in trading scenarios.

## Techniques & Concepts:
- **RSI Calculation**: 
    - Implemented a custom Relative Strength Index (RSI) calculation based on the 14-period average to identify potential buy/sell opportunities.
    - Fine-tuned using a `rsi_tuner` parameter to find the optimal threshold for making trades.
    
- **Price Change Percentage (PC%)**:
    - Calculated the percentage change in stock prices to track trends and determine buying/selling points.
    
- **Trading Strategy Simulation**:
    - Created an algorithm that simulates trades based on the RSI, as well as the conditions of the past few candles (price changes in previous days).
    - Multiple `hold_length_tuner` values were tested to determine the ideal holding period for maximizing profits.

- **Backtesting**:
    - Involves running backtests to simulate how the strategy would have performed over historical data.
    - Tracks metrics such as the percentage of successful trades and total profits across varying scenarios.

- **Parameter Optimization**:
    - Various parameters, such as RSI thresholds and holding periods, were tested and optimized to identify patterns that yield the highest returns.
