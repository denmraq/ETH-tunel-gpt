# ETH Adaptive Probability Tunnel
Static GitHub Pages build. Upload the files directly to the publishing folder (root or docs). No Python/backend.

## Mathematical core
- Forecast anchor: last CLOSED 15m ETH candle; LIVE price is display-only and cannot drag the trajectory.
- ETH price dynamics: short/medium log-return velocity plus acceleration.
- Slow ETH regime: 50D/200D distances and slopes, normalized by realized daily volatility.
- Local standardized displacement (Z): large extensions reduce persistence; it does not mechanically reverse the forecast.
- BTC.D + ETH/BTC + BTC: capital/relative-strength context, never a direct dollar target.
- OI + taker flow + funding: derivatives confirmation inside the radar state; flow is not counted a second time in the trajectory state.
- Adaptive volatility: recent vs previous realized volatility changes P20/P80 expansion.
- P20/P50/P80 and 4h/12h/24h probabilities are samples of ONE continuous 0→24h conditional distribution.

No RSI/MACD/extra indicator stack was added to the trajectory engine. The existing ETH Radar remains a separate current-state signal.

## ONE MATH signal
The headline ETH TUNNEL LONG/SHORT signal is derived from the same continuous 0–24h probability distribution used for the chart and the 4h/12h/24h cards. There is no separate competing Radar headline signal. The internal radar state remains only one market-state input to the mathematical trajectory.
