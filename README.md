# *Long-Run Purchasing Power Parity and the Brexit Effect: Evidence from Portugal-UK Exchange Rates*

Course Project for Advanced Econometrics II

## Research Question

> Did the 2016 Brexit referendum fundamentally alter the long-run equilibrium relationship between GBP/EUR exchange rates and Portugal-UK relative prices?

## Methods
- 📊 Unit root tests with structural breaks (ADF, KPSS)
- 🔗 Cointegration analysis (Engle-Granger & Johansen)
- ⚡ Gregory-Hansen test for cointegration with regime shifts
- ⏳ Vector Error Correction Models (VECM)
- 🚨 Structural break detection (Chow, Quandt-Andrews)

## Data Sources

### Primary Data
| Dataset | Source | Frequency | Period | Key Details |
|---------|--------|-----------|--------|-------------|
| **EUR/GBP Exchange Rate** | European Central Bank | Daily | Jan 1999 - May 2025 | Monthly averages computed from daily spot rates |
| **Portugal Consumer Price Index (CPI)** | Instituto Nacional de Estatística (INE) | Monthly | Jan 1999 - May 2025 | Base - 2012 |
| **UK Consumer Price Index (CPI)** | Office for National Statistics (ONS) | Monthly | Jan 1999 - May 2025 | Base - 2012 |

### Derived Variables
1. **Log Exchange Rate**: `log(euro_per_gbp)`
2. **Log Price Ratio**: `log(cpi_pt) - log(cpi_uk)`
3. **Real Exchange Rate**: `log_exchange_rate - log_price_ratio`
4. **Brexit Dummy**: `post_brexit = 1` for dates ≥ June 2016


