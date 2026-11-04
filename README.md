# moe-craft-models

MOE CRAFT 本機 CPU 執行器（`moe-craft-web/local/engines/cpu`）的模型鏡像倉庫（私有）。

- 模型檔放在 Release 資產（標籤 `models-v1`），檔名、大小、SHA-256、授權與原始出處以主倉庫的 `local/engines/cpu/models.json` 為準。
- 上游（HF／GitHub）可能停更、封存或消失，所以這裡保留一份；每週用 `npm run models:check` 追蹤上游狀態、替代品與本鏡像有無該檔。
- 使用者端安裝只能由介面按「下載並安裝」觸發；執行器以 GitHub 權杖走 API 下載私有資產並核對 SHA-256。
- 各模型授權：anime-segmentation ISNet（Apache-2.0）、BiRefNet（MIT）；重新散布時保留原授權與出處。