# ETH Adaptive Tunnel — Binance Liquidation Magnet Concept

Static GitHub Pages build. No server and no API keys.

## Core
- Binance ETHUSDT futures is the primary market source.
- 15m is used only as the closed-candle ANCHOR, not as the direction motor.
- P50 is one continuous 0–24h mathematical path based on smoothed ETH log-price regression slopes (6h and 13h), acceleration, 50D/200D regime and conditional ETH/BTC relative strength.
- 50D/200D are drawn as thin regime lines and affect P50 only when the slow geometry is materially aligned/displaced.
- ETH/BTC is ignored during ordinary noise and affects P50 only when 4h and 24h relative moves agree and exceed thresholds.
- BTC Dominance is removed.
- OI/taker flow/funding confirm persistence; they do not independently choose LONG/SHORT.

## Liquidation-magnet corridor
The blue boundaries are NOT CoinGlass and NOT actual Binance user liquidation positions. They are estimated potential liquidation clusters derived in-browser from recent Binance Futures price/quote-volume distribution, public OI/taker context and typical leverage-distance assumptions (10x/20x/50x). When P50 consumes a cluster, the boundary selects the next significant estimated cluster.

This is an experimental probabilistic market model, not investment advice.
