交易金額重疊率 (Volume Overlap Ratio, VOR) (主策略-子策略)
      - **公式 (正規化)**：$VOR = \frac{\text{原始重疊率}}{\text{最大可能重疊率}}$
      - **原始重疊率** = $\frac{\sum_t \left( \sum_i x_{it} - \max_i x_{it} \right)}{\sum_t \sum_i x_{it}}$ （其中 $x_{it}$ 為各策略加權金額）
      - **最大可能重疊率** = $\frac{\sum W_{eff, i} - \max(W_{eff, i})}{\sum W_{eff, i}}$ （基於有效資金佔比 $W_{eff}$）
      - **含義**：不同策略在同一時間一起進場的程度。
      - **解讀**：
      - 0%：完全不重疊（兵分多路，進場分散極佳）。
      - 100%：完全重疊（策略高度同步，進場集中）。