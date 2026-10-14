# MP4 影片合併工具

在瀏覽器內合併兩個 MP4 影片，檔案不會上傳到任何伺服器。

線上版：https://wikilee831.github.io/mp4-merger/

- 合併引擎：[ffmpeg.wasm](https://github.com/ffmpegwasm/ffmpeg.wasm)（`@ffmpeg/ffmpeg@0.12.10` + `@ffmpeg/core@0.12.6`，單執行緒版），已內嵌在 `index.html`，可離線使用。
- 編碼相同時直接串接；不同時自動重新編碼（libx264 + AAC）。

## 授權

內嵌的 `@ffmpeg/ffmpeg` 為 MIT 授權；`@ffmpeg/core` 為 FFmpeg（含 x264）的 WebAssembly 版本，採 GPL-2.0-or-later 授權，原始碼見 https://github.com/ffmpegwasm/ffmpeg.wasm 。
