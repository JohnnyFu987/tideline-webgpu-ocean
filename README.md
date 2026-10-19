# Tideline — WebGPU Ocean

一個以 Vibe Coding 完成的互動式海洋場景。作品使用單一 `index.html`，將 CSS、JavaScript、WebGPU shader 與 WebGPU 不支援時的 Canvas fallback 都放在同一個檔案中，適合直接部署到 GitHub Pages。

## 操作方式

- 點擊海面取得操作焦點
- `W/A/S/D`：前後左右移動
- `Q/E`：下降／上升
- `Shift`：加速
- 滑鼠：轉動視角
- `H`：顯示或隱藏控制面板

控制面板可以調整波浪大小、海面起伏、浪尖泡沫與陽光強度，也可以暫停動畫或重設鏡頭。

## 技術重點

- WebGPU 即時渲染
- 多層 Gerstner wave 海面位移
- Fresnel 反射與程序化天空、雲層
- 程序化泡沫與細節法線
- WebGPU 不支援時自動切換 Canvas fallback

GitHub Pages 可直接將此資料夾設定為網站來源，入口檔案是根目錄的 `index.html`。
