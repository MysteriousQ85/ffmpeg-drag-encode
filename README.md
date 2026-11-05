# ffmpeg-drag-encode

Windows 拖拽式 FFmpeg 批量压制工具包

Windows drag-and-drop FFmpeg batch video compressor, auto fallback to NVENC.

## ✨ Features
- Drag video onto `drag_encode.bat` to start compression
- Default: libx265 CRF 23 (great visual quality for archive)
- Auto detect NVENC; use hardware encoder if available
- Batch processing
- Output saved into `output` folder, never overwrite source
- Portable, no installation required

## 📦 Structure

ffmpeg-drag-encode/
├── ffmpeg.exe
├── drag_encode.bat
└── output/

## 🚀 Usage
1. Put `ffmpeg.exe` in the same folder
2. Drag your video file(s) onto `drag_encode.bat`
3. Wait for encoding
4. Find compressed video inside `output`

## ⚙ Preset
- libx265: `-crf 23 -preset medium`
- Audio: AAC 160k stereo
- Fallback to NVENC if GPU encoder is available

## 📜 License
MIT
