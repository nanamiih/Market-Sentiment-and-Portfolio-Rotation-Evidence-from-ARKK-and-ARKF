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
- **FinTech holdings act as a stable core** in both ARKK and ARKF, while most day-to-day portfolio rotation occurs in non-FinTech positions.
- **Sentiment–trading correlations are uniformly weak**, indicating limited mechanical response to same-day news sentiment.
- **ARKK actively adjusts its non-FinTech sleeve**: positive sentiment leads to a statistically significant reduction in non-FinTech exposure on the following day, suggesting this sleeve is used as a shock absorber.
- **ARKF shows weaker and mostly insignificant sentiment-driven rotation**, indicating a more passive tactical structure compared to ARKK.
- **ETF-level sentiment explains less than 1% of daily return variation** and does not support a profitable sentiment-based timing strategy; sentiment is more informative for portfolio rebalancing than for short-term performance prediction.
<img width="1098" height="139" alt="image" src="https://github.com/user-attachments/assets/e7185a6b-a4b3-4df5-9f8d-1c741fa20e82" />
