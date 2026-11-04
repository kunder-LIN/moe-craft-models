# moe-craft-models

MOE CRAFT 本機 CPU 執行器（`moe-craft-web/local/engines/cpu`）的模型鏡像倉庫（公開）。

- 模型檔放在 Release 資產（標籤 `models-v1`），檔名、大小、SHA-256、授權與原始出處以主倉庫的 `local/engines/cpu/models.json` 為準。
- 上游（HF／GitHub）可能停更、封存或消失，所以這裡保留一份；每週用 `npm run models:check` 追蹤上游狀態、替代品與本鏡像有無該檔。
- 使用者端安裝只能由介面按「下載並安裝」觸發；執行器匿名直接下載 Release 資產並核對 SHA-256，不需要任何權杖（2026-11-04 由私有改公開）。
- 只放授權允許再散布的模型，重新散布時保留原授權與出處，檔案不改：

| 資產 | 模型 | 授權 | 原始出處 |
|---|---|---|---|
| `isnetis.onnx` | anime-segmentation ISNet（動漫專用去背） | Apache-2.0 | https://huggingface.co/skytnt/anime-seg ／ https://github.com/SkyTNT/anime-segmentation |
| `birefnet-lite.onnx` | BiRefNet_lite ONNX（通用去背，onnx-community 匯出） | MIT | https://huggingface.co/onnx-community/BiRefNet_lite-ONNX ／ https://github.com/ZhengPeng7/BiRefNet |