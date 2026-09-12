# DeskBeat 🎵 60s Office Ergonomic Rhythm Game

> **60秒辦公室人體工學舒壓節奏遊戲**  
> 專為久坐辦公族打造・開啟鏡頭隨 Lo-Fi 節奏活動眼周、頸椎與雙肩・零隱私風險純本機 AI 運算。

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Technology](https://img.shields.io/badge/AI-MediaPipe-blue)](https://developers.google.com/mediapipe)
[![Audio](https://img.shields.io/badge/Audio-Web%20Audio%20API-orange)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Chrome%20Extension-brightgreen)](#)
[![i18n](https://img.shields.io/badge/Language-English%20%7C%20繁體中文-matcha)](#)

---

## 🌟 核心特色 (Features)

1. **純本機 AI 姿態辨識 (100% Client-side AI)**
   * 基於 Google MediaPipe (FaceMesh & Pose)，所有影像特徵點計算完全在瀏覽器本機端執行。
   * **絕不上傳或儲存任何視訊與個人影像**，辦公室使用安心無虞。

2. **三軌人體工學下落式節奏 (3-Track Ergonomic Rhythm)**
   * 👁️ **眼部活氧軌**：跟隨音符進行左右視線跳動、閉眼深呼吸，舒緩乾眼與螢幕疲勞。
   * 🦒 **頸椎活動度軌**：微幅度左右傾斜牽引頸側肌群，活化僵硬關節。
   * 🧘 **肩胛釋放軌**：自然抬肩（聳肩）與重拍呼氣沉肩，釋放斜方肌緊繃。

3. **動態難度階梯計分與 S 級認證 (Dynamic Scoring & Ranking)**
   * 支援 **低速舒壓 (Easy)**、**中速推薦 (Medium)**、**高速挑戰 (Hard⚡)** 三種梯度。
   * 難度越高得分倍率越高（Hard 3.2x > Medium 1.8x > Easy 1.0x），並結合連續 Combo 加權。
   * 結算依命中率頒發 **S / A / B / C** 綜合工學評級與發光認證。

4. **一鍵社群裂變分享與 1080×1080 成績卡 (Viral Share & Card Export)**
   * 支援行動裝置 Web Share API 原生轉發（LINE, IG, X, WhatsApp, WeChat）。
   * 內建 Canvas 高清繪圖引擎，一鍵生成黑金質感 1080×1080 成果卡片圖片供社群打卡。

5. **全平台響應與多語支援 (Responsive & i18n)**
   * 支援手機直屏（豎屏）、橫屏與電腦寬螢幕，1:1 實體像素自適應，文字永不擠壓。
   * 自動偵測系統語言，支援 **繁體中文 ⇄ English** 即時無縫切換。

6. **Chrome 擴充功能版本 (Manifest V3 Extension)**
   * 支援 Chrome 側邊欄 (Side Panel) 邊工作邊放鬆。
   * 內建久坐番茄鐘定時推播提醒。

---

## 🚀 快速開始 (Quick Start)

### 方式 1：直接透過瀏覽器體驗
打開任何支援 WebRTC 攝影機的現代瀏覽器（Chrome, Safari, Edge），點擊線上連結即可開玩：
👉 `https://43.161.228.192.sslip.io`

### 方式 2：本機運行 (Local Run)
單一檔案架構，無須複雜建置流程：
```bash
# 複製專案
git clone https://github.com/your-username/DeskBeat.git
cd DeskBeat

# 使用任何靜態伺服器啟動 (以 Python 為例)
python3 -m http.server 8080
```
在瀏覽器開啟 `http://localhost:8080` 並允許攝影機存取。

### 方式 3：載入 Chrome 擴充套件 (Chrome Extension)
1. 開啟 Chrome 瀏覽器，進入 `chrome://extensions`。
2. 開啟右上角 **「開發人員模式 (Developer mode)」**。
3. 點擊 **「載入未封裝項目 (Load unpacked)」**，選取 `chrome-extension/` 資料夾。

---

## 🛠️ 技術架構 (Tech Stack)

* **視訊姿態追蹤**：Google MediaPipe (`@mediapipe/face_mesh`, `@mediapipe/pose`)
* **聲音合成引擎**：純原生 Web Audio API (無依賴外部大型音樂檔，自建 Lo-Fi Jazz 合成器)
* **前端框架與佈局**：React 18, Tailwind CSS, HTML5 Canvas 2D
* **擴充規範**：Chrome Extensions Manifest V3 (`sidePanel`, `alarms`, `notifications`)
* **伺服器與部署**：Caddy (HTTPS 自動憑證, HTTP/2, Zstd/Gzip 壓縮)

---

## 🔒 隱私與安全性聲明 (Privacy Policy)

DeskBeat 嚴格恪守使用者資料保護原則：
* **零資料回傳**：攝影機串流畫面只存於本機記憶體，即時分析完即釋放，不傳輸至任何雲端伺服器。
* **無追蹤代碼**：無第三方追蹤器、無廣告、無 Cookie 收集。

---

## 📄 開源授權 (License)

本專案採用 [MIT License](LICENSE) 授權釋出。歡迎自由體驗、Fork、提交 Pull Request 或用於個人健康工作流！
