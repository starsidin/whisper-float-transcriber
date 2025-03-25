# 🎙️ Whisper 悬浮窗语音输入助手
简单的whisper语音转文字（STT）快捷语音输入悬浮窗。本地部署windows版，数据更安全
基于 [OpenAI Whisper](https://github.com/openai/whisper) 的桌面悬浮窗录音转文字工具。它可在任意界面上方悬浮，点击即可开始/结束录音，录音结束后自动识别文字、复制到剪贴板，并以聊天气泡形式显示在窗口中。

推荐使用turbo以上模型，准确率非常高，中英混合输入也非常准确。
turbo模型运行最低配置：显存VRAM=6GB
推荐配置： 显存VRAM<8GB
如果配置无法满足turbo模型，建议使用国内免费大模型（开发中）。

---

## 🚀 功能特性

![1742896337415](https://github.com/user-attachments/assets/805b7edc-8c0d-417d-a9e7-c3dfee018605)

- 🎤 一键悬浮录音
- 🤖 推荐 Whisper 本地模型 ('turbo', `large-v3`)
- 🧠 Whisper 自动识别语音 + 中英混输
- 🔁 自动将繁体转换为简体（使用 OpenCC）
- 📋 自动复制识别结果到剪贴板
- 💬 聊天气泡样式输出识别文字
- 🧩 可在右键菜单中切换模型
- 🌈 无边框、圆角、可拖动、始终置顶悬浮窗

![image](https://github.com/user-attachments/assets/274580f7-42c2-4e82-8be5-b1167c2c1792)

---

## 📦 安装依赖

首先请确保你已安装 Python 3.8+，
然后运行以下命令：

```bash
pip install -r requirements.txt
```
注意：
如果安装失败whisper的安装方法详见官方文档：https://github.com/openai/whisper
whisper必须依赖ffmpeg，在官网下载压缩包后，解压缩并添加到系统PATH中才能正常使用，
安装后在命令行输入ffmpeg弹出版本信息就是安装完成了

## ✅ 使用方法

1. 运行后，会出现一个小型悬浮窗
2. 点击按钮 🎙️ 开始录音 开始说话
3. 再次点击 🛑 停止录音 结束录音
4. 识别结果会显示在界面，并自动复制到剪贴板
5. 右键弹出菜单，可选择模型或关闭程序
￼
## 💡 注意事项
• 默认使用 GPU（若可用），否则回退到 CPU
• 模型将自动下载缓存到本地（首次运行可能稍慢）
• 若需更高准确率，可切换为 large-v3 模型（需要较高显存）

## ✅ 即将添加的功能 | Coming Soon
🧠 支持其他模型

⌨️ 添加快捷键支持（如 F9 开始/停止）
Global hotkey support (e.g., F9 to start/stop recording)

📌 支持粘贴到目标应用（如微信、Word）
Auto-paste to target apps (e.g., WeChat, Word)

📜 历史记录窗口（可查看并复制以前的识别结果）
Recognition history viewer (view/copy past results)

☁️ 模型 API 模式（轻量版，无需本地模型）
Cloud-based Whisper API option for lightweight use


## 欢迎大家开发想要的功能，或对需要的功能进行留言
