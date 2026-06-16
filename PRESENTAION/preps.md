HEre will be my presentation
This is a simple analysis I’ve put together on LVMH shares in 2010-2023. We’ll be looking at four key areas: returns, risk, market performance and profit drivers.
Before the formal analysis, we performed rigorous data cleaning using Python. As LVMH is traded in Paris and the S&P 500 in New York, the public holidays in the two countries are entirely different. 

One of the core pieces of logic in our code utilises Pandas’ `dropna()` function to remove all days when the markets were closed on both sides, ensuring that every subsequent daily comparison is conducted under exactly the same conditions. This is the first step in quantitative financial analysis.”
“First, let’s look at long-term returns. In our code, we used pct_change() to calculate daily price movements, then use cumprod()—the ‘cumulative product’—to simulate the effect of compounding.

 The results were astonishing: from early 2010 to the end of 2023, LVMH’s total return reached a staggering 1,112.44%! What does this mean in practical terms? If you had used the money to buy a basic LV handbag in early 2010 to purchase its shares instead, by the end of 2023 you would have had 12 handbags. Its annualised return was as high as 19.54%, almost on a par with the long-term average return of the ‘Oracle of Omaha’, Warren Buffett.

Finance teaches us that high returns inevitably come with high risk. We use the statistical concept of ‘standard deviation’ to measure volatility. Multiplying by the square root of 252 converts daily volatility into the internationally recognised annualised volatility. LVMH’s overall annualised volatility stands at 27.10%, indicating that it is not a steady stock, but rather a thrilling one.

As can be clearly seen from the purple ‘rolling volatility chart’ we have generated, when the COVID-19 pandemic broke out in early 2020 and physical shops around the world were forced to close, investor panic caused the share price to swing wildly, with short-term rolling volatility surging instantly to over 60 per cent! This tells us that to achieve the 11-fold return mentioned earlier, you must possess strong mental resilience to weather the darkest moments of such significant drawdowns in the asset’s value.”

We have compared it against the world’s most authoritative index, the S&P 500. Using code, we have ‘normalised the starting point’, which means we have assumed that on the first day of 2010, you invested £1 each in the S&P 500 and LVMH.

As you can see, whilst the S&P 500 has also performed well over the past decade or so, LVMH has followed a completely independent trajectory. Particularly since 2016, as global luxury consumption has upgraded, LVMH has pulled decisively ahead of the broader market. Even during the 2020 pandemic, when it fell more sharply than the broader market, its rebound was far faster and more substantial than that of the broader market, thanks to its exceptionally strong brand premium.”
