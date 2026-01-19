# Market Sentiment and Portfolio Rotation Evidence from ARKK and ARKF
This project studies how actively managed ETFs — **ARK Innovation ETF (ARKK)** and **ARK FinTech Innovation ETF (ARKF)** — adjust their portfolio holdings and performance in response to market news sentiment. Using daily ETF holdings, financial news headlines, and NLP-based sentiment analysis (FinBERT), the project examines whether sentiment affects **portfolio rotation behavior** and **short-term returns**.

### Key Variables
| Variable          | Description                                                                          |
| ----------------- | ------------------------------------------------------------------------------------ |
| `Sentiment_t`     | Daily aggregated news sentiment score (positive − negative), generated using FinBERT |
| `Return_t`        | Daily percentage return of ARKK or ARKF                                              |
| `Weight_Change_t` | Daily change in portfolio allocation (%)                                             |
| `Trade_Event_t`   | Binary indicator of significant trading activity (> 1% weight change)                |

### Key Outcomes
- FinTech holdings behave as stable core positions with near-zero sensitivity to sentiment.
- Non-FinTech holdings act as a tactical “satellite sleeve”, especially in ARKK, absorbing sentiment shocks through rebalancing.
- Sentiment explains less than 1% of daily ETF return variation for both ARKK and ARKF.
- A simple sentiment-based trading strategy does not outperform buy-and-hold.
- Market sentiment is more informative for portfolio composition decisions than for predicting ETF performance.
