# 🎙️ Whisper 悬浮窗语音输入助手
简单的whisper语音转文字（STT）快捷语音输入悬浮窗。本地部署windows版，数据更安全
基于 [OpenAI Whisper](https://github.com/openai/whisper) 的桌面悬浮窗录音转文字工具。它可在任意界面上方悬浮，点击即可开始/结束录音，录音结束后自动识别文字、复制到剪贴板，并以聊天气泡形式显示在窗口中。

---

## 🚀 功能特性

- 🎤 一键悬浮录音
- 🤖 支持 Whisper 本地模型 (`tiny`, `base`, `small`, `medium`,'turbo', `large-v3`)
- 🧠 Whisper 自动识别语音 + 中英混输
- 🔁 自动将繁体转换为简体（使用 OpenCC）
- 📋 自动复制识别结果到剪贴板
- 💬 聊天气泡样式输出识别文字
- 🧩 可在右键菜单中切换模型
- 🌈 无边框、圆角、可拖动、始终置顶悬浮窗

---

## 📦 安装依赖

首先请确保你已安装 Python 3.8+，然后运行以下命令：

```bash
pip install -r requirements.txt
