# 超級循環

一個單頁的模擬遊戲：從 2026 年 11 月走到 2027 年底，一則一則決定事件的結果，看 AI 與科技市場這一波落在哪裡。每一步都給出各種結局的機率，以及各標的的價格與日 K。

## 怎麼用

用瀏覽器打開 `index.html` 即可，不需要安裝、不需要伺服器（圖表函式庫已內嵌在同一個檔）。放在網站上時，頁面開啟會向同一個網站讀一個小檔 `version.json`，看有沒有新版；不送出任何資料，讀不到就照常使用。

## 資料與方法

世界由一組狀態（例如地緣緊張、利率方向、AI 需求、資金壓力）與事件組成。每一天，排定的事件照公開日程發生，突發事件照依處境調整的發生率發生；事件的結果改變狀態，狀態再影響之後事件的機率，所以同一個起點會走出不同的路徑。價格由市場模型照事件與狀態的變化算出。數值的依據來自公開資料與寫明的判斷；模型仍在逐步更新。

## 第三方元件與授權

- TradingView Lightweight Charts™ 5.3.0（[原始碼](https://github.com/tradingview/lightweight-charts)），Copyright (c) 2026 TradingView, Inc.，Apache License 2.0，全文見 `licenses/LICENSE-lightweight-charts.txt`。圖表由 TradingView 的 Lightweight Charts 繪製。
- [technicalindicators](https://github.com/anandanand84/technicalindicators) 3.1.0，Copyright (c) 2016 Anand Aravindan，MIT License，全文見 `licenses/LICENSE-technicalindicators.txt`。
