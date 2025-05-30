
# 🎨 藝術名畫辨識器

使用 OpenAI 的 CLIP 模型來辨識知名畫作，並透過 Google 語音合成（gTTS）提供中文語音解說。

## 📌 功能介紹

- 📷 **圖像辨識**：上傳一張畫作圖片，系統會比對內建資料庫，自動判斷是誰的作品。
- 🗣️ **中文語音導覽**：自動產生語音講解畫作背景與藝術家資訊。
- 🌐 **支援 Colab 執行**：無需安裝，可直接使用 Google Colab 執行完整功能。

---

## 🚀 快速開始（建議使用 Google Colab）

👉 [點此開啟 Colab 執行](https://colab.research.google.com/github/你的帳號/你的Repo/blob/main/art_identifier.ipynb)

1. 點選 `Run All`（執行全部）
2. 上傳任意知名畫作圖片（如：Mona Lisa、Starry Night 等）
3. 系統將顯示畫作資訊並自動播放中文語音講解

---

## 🖼️ 支援的畫作範例

| 畫作名稱 | 藝術家 | 年代 |
|----------|--------|------|
| 蒙娜麗莎 (Mona Lisa) | 達文西 | 1503–1506 |
| 星夜 (Starry Night) | 梵谷 | 1889 |
| 吶喊 (The Scream) | 孟克 | 1893 |
| 親吻 (The Kiss) | 克林姆 | 1907–1908 |
| 格爾尼卡 (Guernica) | 畢卡索 | 1937 |

完整列表請見程式中的 `known_paintings` 字典。

---

## 📁 專案結構

```
my-art-identifier/
├── art_identifier.ipynb   # Colab 版程式碼（辨識 + 語音）
├── index.html             # 上傳圖片展示網頁（靜態用）
└── README.md              # 使用說明文件
```

---

## 🔧 技術架構

- OpenAI CLIP 模型（`ViT-B/32`）
- PyTorch
- gTTS（Google Text-to-Speech）
- PIL / IPython.display
- Google Colab / GitHub Pages

---

## 📌 注意事項

- **index.html 為純前端頁面**，無法進行模型辨識與語音播放，僅用於展示 UI。
- 若需完整功能，請透過 Colab 運行 `art_identifier.ipynb`。

---

## 📜 授權 License

本專案僅供教育用途，如需商業使用請自行確認各模型與資源授權條款。
