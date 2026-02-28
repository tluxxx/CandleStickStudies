# CandleStickStudies
In this repository I will collect some studies on candle-stick patterns. The principal content of the notebooks is as follows: 
* candlestick_studies_00_talib.ipynb:
  * In this noteboook we will demonstrate how to use the library TA-Lib to detect candlestick-patterns in stock data (using Colab).
  * see blog https://medium.com/@Tobi_Lux/using-ta-lib-for-detecting-candle-stick-patterns-in-stock-prices-04384dcbe8ab for details NOTE: meanwhile TA-Lib has moved to GitHub. This enables a much cleaner approach, the notebook was therefore adapted. 
* 01_candlestick_studies_predictive_power_01.ipynb:
  * Topics of the study are:
    * frequency of occurance of candlestick-patterns in real stock data (S&P-500 index from 2000 to mid 2024)
    * identification of the "most-active"-patterns (by highest number of occurences)
    * analyses of the development of cummulated return over time (1-20 days after occcurence of a pattern)
    * identification of the most profitable patterns
    * analysing distribution of returns over time, test for normality
    * comparison trading of most profitable candlestick patterns with trading, based on completely random entries; statistical tests of return distributions
  * The content of the notebook was published in the blog: https://medium.com/@Tobi_Lux/on-predictive-power-of-candlestick-patterns-in-stock-trading-an-experiment-d71dd92b4b27
* 01_candlestick_studies_predictive_power_updated_02.ipynb
  * Topics are: 
    * Analyzing S&P 500 data from 2000 to 2025 for candlestick patterns using TA-Lib, generating bullish and bearish pattern signals
    * Introducing a simple EMA-based trend filter (and studying the impact)
    * Counting bullish/bearish signals and identifying the most active patterns
    * For each detected pattern (event/signal), compiling key information as date of occurrence, mode (bullish, bearish), market trend (no filter, up-trend, down-trend) and cumulative returns for the 20       days following the signal
    * Analyzing the distribution of cumulative returns
    * Rigorous statistical testing for:
      * Mean cumulative returns after a pattern signal vs. mean cumulative returns after random entries
      * Win rate after a pattern signal vs. win rate after random entries
  * The content of the notebook was published in the blog xxxxxxxxxx
  
* 01_candlestick_studies_test_for_equal_means:
  * The notebook perfrms different statistical teas for equal means on model distributions (Gamm-Distribution, exponential distribution
  * Focus is the explanation of the permutation test and the codeing of the test using different methods (from direct loops to vectorisation, further speed optimisation until a fully fledged numbe version of the code that ist ultra fast. The lase version is also used in the notebok: 01_ candlestick_studies_predictive_power_updated_01.ipynb    
